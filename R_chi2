#Import the dataset


# Hypotheses:
# Null hypothesis = color is not related to obesity
# Alternative hypothesis = color is related to obesity



# check the data
str(mice)

# change the format of the variables 
mice$color = factor(mice$color,
                    levels = c(0,1),
                    labels = c('white', 'black'))

mice$obese_yes = factor(mice$obese_yes,
                        levels = c(0,1),
                        labels = c('normal', 'obese'))


# Chi2 test:
# -- assumptions: expected frequencies >= 5
table(mice$color, mice$obese_yes)

chisq.test(mice$color, mice$obese_yes, correct = FALSE)$expected

test1

#p > .05 --> color is not related to obesity


#Fisher's exact test
fisher.test(mice$color, mice$obese_yes)

# p > .05 -> color is not related to obesity

# p = .012 -> color is related to obesity



