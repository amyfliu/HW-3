# Hw3
# Grade point average
#
gpa.df <- read.table("CH01PR19.txt",header=FALSE)
names(gpa.df) <- c("gpa","act")
attach(gpa.df)
fit1 <- lm(gpa ~ act,data=gpa.df)
summary(fit1)
# Critical constant for 95 percent CI for beta_1
cc <- qt(.975,118); cc



#  Extra practice (not on Hw3)
#  Get confidence interval for muY for act=28
#  and prediction interval for individual Y for act=28
nd <- data.frame(act=28)
predict(fit1, newdata=nd,level=.95,interval="confidence")
predict(fit1, newdata=nd, level=.95, interval="prediction")
anova(fit1)
