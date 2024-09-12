# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Two-stage polytomous logistic regression Use TwoStageModel (TOP) With (In) R Software
install.packages("remotes")
remotes::install_github("andrewhaoyu/TOP")
library("TOP")
TOP = read.csv("https://raw.githubusercontent.com/timbulwidodostp/TOP/main/TOP/TOP.csv",sep = ";")
# Estimation Two-stage polytomous logistic regression Use TwoStageModel (TOP) With (In) R Software
ODS <- data[,1:4]
SNP <- data[,6]
PC1 <- data[,7]
TOP_1 <- TwoStageModel(y=ODS,additive=cbind(SNP,PC1), missingTumorIndicator = 888)
TOP_1
TOP_2 <- TwoStageModel(y=ODS,baselineonly = SNP, additive=PC1, missingTumorIndicator = 888)
TOP_2
# Two-stage polytomous logistic regression Use TwoStageModel (TOP) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished