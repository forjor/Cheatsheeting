
# Validation

## Value is within set.
```terraform
  validation {
    condition     = contains(["full-tf", "full-ui"], var.management_strategy)
    error_message = "Valid values for var: test_variable are (full-tf, full-ui)."
  }
```
