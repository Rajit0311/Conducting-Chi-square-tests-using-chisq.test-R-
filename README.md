# Conducting-Chi-square-tests-using-chisq.test-R-
- A Chi-square test is a statistical method used to determine whether there is a significant association between categorical variables.

CODE:-
# Create a contingency table
transport <- matrix(c(30, 20,
                      15, 35),
                    nrow = 2,
                    byrow = TRUE)

# Add row and column names
dimnames(transport) <- list(
  Gender = c("Male", "Female"),
  Transport = c("Car", "Bike")
)

transport
# Perform chi-square test
chi_result <- chisq.test(transport)

# Display result
chi_result
