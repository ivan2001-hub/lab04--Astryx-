# lab04--Astryx-
# Lab 4 — Automated Software Testing

## Group Name
## Gp name - Astryx 
## Kaung Htet Wai(Argon) - 6805140029
## Bhone Myat Kyaw(Ivan) - 6805140041
## Chan Myae Myae Zaw(Coe) - 6805140032
## Thazin Phyu (Diana) - 6805140023

**Astryx**


## Who Did What

| Member | GitHub Username | File |
|---|---|---|
| Member A | ivan2001-A | `test_deposit.py` |
| Member B | Chanmmzaw-B | `test_withdraw.py` |
| Member C | kaunghtetwaiargon-C | `test_teardown.py` |
| Member D | phyu-19-D | `test_shared.py` |
| Member E | Ivan-E | `conftest.py` |

## Our Merge Conflict

During Round 3, each group member edited the same section of `README.md` at roughly the same time. Because the members made different changes to the same part of the file, Git could not automatically decide which version should be kept.

The conflict markers we encountered were:

```text
| Member A | ivan2001-A | test_deposit.py |
| Member B | Chanmmzaw-B | test_withdraw.py |
```

The final version kept both members' rows, along with the rows for the other group members:

```text
| Member A | ivan2001-A | test_deposit.py |
| Member B | Chanmmzaw-B | test_withdraw.py |
| Member C | kaunghtetwaiargon-C | test_teardown.py |
| Member D | phyu-19-D | test_shared.py |
| Member E | ivan2001-E | conftest.py |
```

Git could not resolve the conflict automatically because both versions changed the same section of `README.md`. Git therefore required us to manually decide which changes should remain.

After resolving the conflict, we removed all conflict markers and committed the resolved file.

## Git Contribution Summary

Run:

```bash
git shortlog -sn
```

Paste the actual output below:
    10  Ivan
     2  Coe
     1  Argon
     1  Thazin Phyu
     1  ivan2001-hub


All group members should appear in the contribution summary.

## Reflection Questions

### 1. Why was your push rejected, and how did you fix it?

My push was rejected because another group member had pushed changes to GitHub before me, so my local repository was no longer up to date. I fixed it by running `git pull` to get the latest changes and then running `git push` again.

### 2. Why could Git not resolve the README conflict automatically?

Git could not resolve the conflict because multiple group members changed the same part of the `README.md` file. Git could not automatically determine which changes should be kept, so we had to manually resolve the conflict.

### 3. What is the difference between committing and pushing?

Committing saves a snapshot of our changes in the local Git repository. Pushing uploads those commits to the shared GitHub repository so that other group members can see them.

### 4. How do fixtures reduce duplicated setup code in tests?

Fixtures allow us to create common test setup code once and reuse it across multiple tests. For example, instead of creating a new `BankAccount(100)` inside every test, we can create an `account` fixture and pass it into the tests that need it.

## Final Verification

Before submitting, we checked that:

- All group members contributed to the repository.
- Every member has commits correctly attributed to them.
- All required test files are present.
- `pytest -v` passes successfully.
- The README contains all required sections.
- No Git merge conflict markers remain.
- The repository is public.

## Repository

**GitHub Repository:**  
[https://github.com/ivan2001-hub/lab04--Astryx-]