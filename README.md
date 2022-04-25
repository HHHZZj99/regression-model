# regression-model
#y=-32.08+45.92x
# x:7  ,3, 4, 6,  10, 9
# y:276,43,82,136,417,269
>model<-lm(y~x)
>model

call:
lm(formula=y~x)

Coefficients:
(Intercept)        x
-32.08             45.92

>coefs<-coef(model)
>plot(x,y,pch=20,col="red",xlab="Number new friends",ylab="Time spent (seconds)")
>abline(coefs[1],coefs[2])
