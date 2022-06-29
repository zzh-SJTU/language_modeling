main_bay.py 为通过贝叶斯优化（为了节省时间只设置了训练6个epoch）调整超参数，该文件里有详细的代码注释，请助教评测代码可读性时参考该文件。
需要安装 bayesian-optimization == 1.2.0
python  python main_bay.py--cuda --emsize 1250 --nhid 1250 --tied 来进行贝叶斯优化调整超参数

main.py 为助教提供的baseline
通过 python main.py --cuda --emsize 1250 --nhid 1250 --dropout 0.4 --epochs 40 --tied 来复现PPL = 112.54的实验结果（模型为model.pt）