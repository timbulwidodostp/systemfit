# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Linear Estimation (Estimating) Systems of Simultaneous Equations Use systemfit With (In) R Software
install.packages("systemfit")
library("systemfit")
systemfit = read.csv("https://raw.githubusercontent.com/timbulwidodostp/systemfit/main/systemfit/systemfit.csv",sep = ";")
# Estimation Linear Estimation (Estimating) Systems of Simultaneous Equations Use systemfit With (In) R Software
eqDemand <- consump ~ price + income
eqSupply <- consump ~ price + farmPrice + trend
system <- list(demand = eqDemand, supply = eqSupply)
systemfit <- systemfit(system, data=systemfit)
summary(systemfit)
# Linear Estimation (Estimating) Systems of Simultaneous Equations Use systemfit With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished