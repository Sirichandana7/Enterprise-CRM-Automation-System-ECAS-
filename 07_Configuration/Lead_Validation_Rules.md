# Lead Validation Rules

## Rule 1: Budget Must Be Positive

**Business Requirement**

If a Budget is entered, it must be greater than zero.

**Formula**

```text
AND(
    NOT(ISBLANK(Budget__c)),
    Budget__c <= 0
)
```

**Error Message**

Budget must be greater than zero.
