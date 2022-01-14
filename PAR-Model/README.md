# **P**ay **A**ttention when **R**equired (PAR) Transformer-XL


An implementation of the Pay Attention when Required transformer from the paper: https://arxiv.org/pdf/2009.04534.pdf

Reference github: https://github.com/Jmkernes/PAR-Transformer-XL

Mô hình mặc định mà chúng tôi sử dụng có độ dài bộ nhớ 16, feed-forward dimension 512, attention dimension 128 và 6 stochastic blocks, với một lớp adaptive softmax  và 2 cụm. Chúng tôi đã đào tạo trên GPU colab trong 20 epoch, mất tổng cộng 23 phút 13 giây. Sử dụng Adam optimzer với p cosine rate decay: warmup ban đầu là 4000 bước và learning rate tối đa là 1e-4, giảm dần về 0 khi kết thúc quá trình đào tạo.
