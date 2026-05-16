````md
# Day 6 — Triggers & SOQL

## 1. What is SOQL?
SOQL (Salesforce Object Query Language) is used to retrieve data from Salesforce objects like Account, Contact, Lead, and Opportunity.

Example:
```sql
SELECT Name, Phone FROM Account
````

---

## 2. What is an Apex Trigger?

An Apex Trigger is Apex code that runs automatically when records are inserted, updated, deleted, or undeleted.

Example:
When an Opportunity becomes “Closed Won”, automatically create a follow-up task.

---

## 3. Difference

### Flow vs Trigger

| Flow                       | Trigger                      |
| -------------------------- | ---------------------------- |
| Declarative                | Programmatic                 |
| Drag-and-drop              | Apex code                    |
| Easier for admins          | Used for complex logic       |
| Best for simple automation | Best for advanced automation |

### Before vs After Trigger

| Before Trigger                    | After Trigger                 |
| --------------------------------- | ----------------------------- |
| Runs before save                  | Runs after save               |
| Used for validation/field updates | Used for related records      |
| Faster                            | Used when record ID is needed |

---

## 4. Trigger Use Cases

1. Auto-copy billing address to shipping address
2. Create follow-up task after Closed Won Opportunity
3. Prevent Account deletion with related Opportunities
4. Notify manager when high-priority Lead is created
5. Create onboarding tasks for new customers

---

## 5. Query Examples

```sql
SELECT Name FROM Account WHERE BillingCity='Hyderabad'
```

```sql
SELECT Name, Amount FROM Opportunity WHERE StageName='Closed Won'
```

```sql
SELECT Name FROM Contact WHERE LastName='Smith'
```

---

## 6. Reflection

Enterprise systems react automatically to data changes using triggers and automation.
This improves:

* Speed
* Accuracy
* Consistency
* Customer experience

---

# Reflective Questions

### 1. Why do systems need triggers?

To automate actions instantly and reduce manual work.

### 2. Difference between polling and event-driven systems?

Polling checks repeatedly.
Event-driven systems react instantly when events happen.

### 3. Why are database queries important?

Queries help retrieve exact business data efficiently.

### 4. When should Flows be preferred over Triggers?

When automation is simple and doesn’t require complex coding.

### 5. What problems happen if automation becomes too complex?

Slow performance, debugging issues, and maintenance problems.

### 6. Why should developers think carefully before automating?

Bad automation can create wrong data and break workflows.

---

# End of Day Outcome

I now understand:

* SOQL queries
* Apex Triggers
* Event-driven systems
* Flow vs Trigger
* Enterprise automation concepts

```
```

