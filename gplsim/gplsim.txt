# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Generalized partially linear single index models Use gplsim With (In) R Software
# Spline Estimation for Generalized partially linear single index models (GPLSIM) Use gplsim With (In) R Software
install.packages("gplsim")
library("gplsim")
gplsim = read.csv("https://raw.githubusercontent.com/timbulwidodostp/gplsim/main/gplsim/gplsim.csv",sep = ";")
# Estimation
# Generalized partially linear single index models Use gplsim With (In) R Software
# Spline Estimation for Generalized partially linear single index models (GPLSIM) Use gplsim With (In) R Software
y=gplsim$ozone
X=as.matrix(gplsim[,c(4,5,3)])
colnames(X)=colnames(gplsim[,c(4,5,3)])
Z=NULL
gplsim <- gplsim(y,X,Z=NULL,family = gaussian,bs="ps")
summary(gplsim)
plot_si(gplsim,yscale=c(1,6),plot_data = TRUE)
# Generalized partially linear single index models Use gplsim With (In) R Software
# Spline Estimation for Generalized partially linear single index models (GPLSIM) Use gplsim With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished