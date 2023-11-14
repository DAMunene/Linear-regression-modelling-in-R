# linear-regression-modelling-in-R
# Sample data
data <- data.frame(
  X = c(1, 2, 3, 4, 5),
  Y = c(3, 5, 7, 9, 11)
)

# Fit a linear regression model
linear_model <- lm(Y ~ X, data = data)

# Display summary statistics of the linear model
summary(linear_model)

# Make predictions using the linear model
new_data <- data.frame(X = c(6, 7, 8))
predictions <- predict(linear_model, newdata = new_data)

# Display predictions
cat("Predictions:\n")
print(predictions)
