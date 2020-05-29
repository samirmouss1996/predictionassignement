#Dataset
traindata = "training.csv" testdata = "testing.csv"
train <- read.csv(traindata, sep=",", header=TRUE, na.strings = c("NA","",'#DIV/0!')) test <- read.csv(testdata, sep=",", header=TRUE, na.strings = c("NA","",'#DIV/0!'))

#Remove NA AND 0
train <- train[, colSums(is.na(train)) == 0] test <- test[, colSums(is.na(test)) == 0] dim(train)


library(dplyr) classe = train$classe train[, numer]= train <- mean_s <- train std_s <- train meanToSd <- train names(train)

mean_s <- mean_s %>% group_by(classe) %>% summarise_all(funs(mean)) std_s <- std_s %>% group_by(classe) %>% summarise_all(funs(sd)) mean_to_sd <- function(x){mean(x)/sd(x)} meanToSd <- meanToSd %>% group_by(classe) %>% summarise_all(funs(mean_to_sd)) meanToSd
