# AI In Public

In order to ramp up in my practical and theoretical foundation in AI, I am adding a tracker to track my progress in learning. The focus will be on LLMs. 

# Objective
1. Be able to explain in both high and low-level how an LLM works
1. Be able to explain the latest innovations in LLMs training and inference and what those changes brought
1. Be able to implement a basic LLM from scratch
1. Be able to deconstruct an open-source LLM model to it's components and build it back up
1. Master PyTorch first (due to available resources) then master Jax and T5X

# Daily Progress
## Sunday, 20 July 2025
1. Read [UL2 Paper](https://arxiv.org/abs/2205.05131)
   1. Decoder-only, Encoder-only, Encoder-Decoder architectures
      1. Encoder-Decoder very similar to Decoder-only but Encoder-Decoder is more sparse
   2. Input-to-target paradigm vs in-place paradigm (Masked Language Modeling)
   3. Mixture of Denoisers
   4. Sparse models
   5. Pre-training objectives - CausalLM, PrefixLM, Span Corruption (T5)
   6. R-denoiser, S-denoiser, X-denoiser
1. Watched [CS336 Lecture 1: Overview and Tokenization](https://www.youtube.com/watch?v=SQ3fZ1sAqXI&list=PLoROMvodv4rOY23Y0BoGoBGgQ1zmU_MT_&ab_channel=StanfordOnline)
   1. BPE tokenization - find most frequenct char pairs and group them together N number of times

## Monday, 21 July 2025
1. Watched [CS336 Lecture 2: Pytorch, Resource Accounting](https://www.youtube.com/watch?v=msHyYioAyNE&list=PLoROMvodv4rOY23Y0BoGoBGgQ1zmU_MT_&index=2&ab_channel=StanfordOnline)
2. Started working on [Assignment 1](https://github.com/limyifan1/assignment1-basics) on creating a BEP tokenizer

## Tuesday, 22 July 2025
1. Continued [Assignment 1](https://github.com/limyifan1/assignment1-basics) on creating a BEP tokenizer
2. Managed to get 2 out of 3 tests passed
3. Failing on the speed test due to very naive implementation, will work on optimizing the speed tomorrow
4. Learnt all about pretokenization, UTF-8 format (not all 1 byte), converting to bytes, cProfile to profile code

## Thursday, 24 July 2025
1. Working on optimizing BEP tokenizer to pass all 3 tests

## Friday, 25 July 2025
1. Managed to optimize the BEP tokenizer to make it faster and pass all 3 tests

## Saturday, 25 July 2025
1. Working on get_tokenizer which will take an existing vocab and merges and encode/decode strings
2. Completed the encode, working on decode
