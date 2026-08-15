[README.md](https://github.com/user-attachments/files/31102625/README.md)
# Health ad copy check

A Claude skill that audits ad copy for healthcare and wellness advertisers against Google's personalized advertising policy for health and Meta's personal attributes policy, flags what risks disapproval, and rewrites it.

Built by [Builders](https://at.builders), a fully remote creative and paid growth agency. Build your brand, build your audience, grow.

---

## The problem it solves

Health advertisers get copy rejected for one reason more than any other: the ad speaks to the reader as if it knows their medical condition. Google calls it the personalized advertising policy for health. Meta calls it personal attributes. Same underlying test, different names.

The rule turns on framing, not topic. The same condition can appear in copy that passes and copy that fails:

| Fails | Passes |
|---|---|
| Find Out Why You're In Pain | Chiropractic Care For Neck & Back Pain |
| Headaches Keep Coming Back? | Care For Recurring Headaches |
| Are You Diabetic? | Diabetes Care And Support |
| Relieve Your Pain For Good | Long-Term Pain Relief |

The distinction is whether the copy asserts the reader has the condition, or describes what the advertiser treats. Easy to state, easy to break, and it costs you approved assets in an RSA when you get it wrong.

## What it does

Paste headlines, long headlines, descriptions, or primary text. Get back:

- Which assets fail, which are borderline, which are clear
- The exact phrase causing the problem
- A compliant rewrite that stays within the character limit
- Character-limit violations flagged in the same pass

It also distinguishes copy problems from account-level restrictions — when every asset in an account is flagged, including neutral ones like the business name, that's the account's health classification and no rewrite lifts it. Knowing the difference saves you rewriting copy that was never the issue.

## Covers

**Google Ads** — personalized advertising policy for health, account-level restriction behaviour, RSA and PMax character limits.

**Meta** — privacy violations and personal attributes, the "other" trigger, family attribution, negative self-perception, before/after and problem-area creative rules, unsubstantiated claims.

## Install

Download **`health-ad-copy-check.skill`** and add it in Claude under Settings → Capabilities.

That single file contains everything. Once installed it loads automatically whenever you're working on health or wellness ad copy — no command needed. Paste your assets and ask for an audit, or just ask for headlines and the rules get applied as they're written.

The unpacked source is in `health-ad-copy-check/` if you want to read or edit it before installing.

## Example

```
Audit these headlines for a physiotherapy clinic:

Tired Of Your Back Hurting?
Expert Physical Therapy
Are You Living With Chronic Pain?
Same-Day Appointments
```

Returns a table marking the first and third as failures, with rewrites, and the second and fourth as clear.

## Notes

This encodes published platform policy and practical experience applying it. It is not legal advice, and platform policies change — treat it as a first-pass filter that catches the common failures, not a guarantee of approval.

Suggestions and corrections welcome via issues.

---

Built by [Builders](https://at.builders) — build your brand, build your audience, grow.
