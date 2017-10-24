# Simple, straight-forward implementation of CycleGAN in PyTorch

Recently I read the <a href="https://arxiv.org/abs/1703.10593">CycleGAN paper</a> and I was absolutely fascinated! Zebras turning into horses and paintings turning into photos seemed (and still does) magical.

Along with all their amazing results, you can even find the code on their <a href="https://junyanz.github.io/CycleGAN/">project page</a>. Reading and understanding the code, however, is a pain in the ass; its got too many files and is far too complicated at times (try it once!). So, I chucked that and implemented this jupyter notebook while directly referring to the original paper.

The notebook, however, was not run for more than 10 epochs because I currently do not have access to a good GPU (still saving up for that!). Hope you have a better experience than me and I'm excited to see your results!

## Some changes to the original paper:

I added 2 discriminators for every generator. One of the discriminators works on 70x70 patches (as mentioned in the paper) and the other looks at the whole image. Later I aggregate the scores of both these discriminators for a better result. 

## TODO

Adding linear learning-rate decay if it is trained for more than 100 epochs.
