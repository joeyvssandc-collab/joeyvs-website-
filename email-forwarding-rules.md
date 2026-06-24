# Email Forwarding Rules

## Rule 1 — AI (broad match)

**Trigger:** The word `AI` appears anywhere in the email — subject, body, or sender address/name.

**Action:** Forward to AIGURU110.

**No keyword list.** Any email that contains the string "AI" (case-sensitive) in any field is forwarded. This replaces the previous approach of maintaining a specific list of AI-related keywords.

---

## Rule 2 — Etsy (keyword-based)

**Trigger:** The email matches one or more of the following keywords in the subject or body:

- `Etsy`
- `order confirmed`
- `your order`
- `shipped`
- `delivery`
- `tracking`
- `listing`
- `shop`

**Action:** Forward to AIGURU110.

**Why keyword-based?** Generic terms like `shop` or `listing` appear in many unrelated emails. Matching only when combined with Etsy-specific context prevents false positives.

---

## Deduplication

If an email matches both Rule 1 and Rule 2, it is forwarded **once**. No duplicate forwards.

---

## Summary

| Rule | Match method | Field scope | Destination |
|------|-------------|-------------|-------------|
| AI   | Broad — any occurrence of "AI" | Subject, body, sender | AIGURU110 |
| Etsy | Keyword list | Subject, body | AIGURU110 |
