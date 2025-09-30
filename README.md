# Cybersecurity-6-Password-Security
Outcome: Understanding password security and best practices. Key Concepts: Password strength, brute force attack, dictionary attack, authentication, best practices.
 Strong Password Evaluation Report (Fully Documented)

## I. Executive Summary
An investigation was conducted using 10 distinct password examples for password security analysis. The password strength was checked on www.passwordmeter.com and observations recorded and analysed in this report. The evaluation of ten distinct password strategies confirmed that Length is the single most dominant factor in password strength, providing an exponential increase in security (entropy). While Complexity (mixing character types) is necessary to avoid easy cracking, it cannot compensate for a short length. The strongest passwords achieved a perfect 100% score by combining maximum length (16+ characters) with high randomness (zero sequence or consecutive character deductions).

## II. Password Strength Evaluation Results
| Conceptual Password Used | Length (Chars) | Composition | Score (%) | Complexity | Key Insight Demonstrated |
| :--- | :--- | :--- | :--- | :--- | :--- |
| soccer | 6 | Lowercase Only | 6% | Very Weak | Baseline: Short length + single character set is catastrophic. |
| Socc3r | 6 | Upper/Lower/Number | 38% | Weak | Mixing character types (Complexity helps) but cannot overcome short length. |
| password1234 | 12 | Lowercase/Number | 50% | Good | Length is dominant (raised score), but the use of common dictionary words and number sequences severely limits security. |
| P@$$wOrd!9 | 9 | All 4 Types | 96% | Very Strong | Demonstrates the power of high randomness and all character types, achieving a near-perfect score at moderate length. |
| myfavoritedogisnamedrocky | 25 | Lowercase Only | 26% | Weak | Isolates the Length Penalty: Even extreme length (25 chars) is heavily penalized if it's only one character type (-25 for "Letters Only"). |
| j2#Xz6!7 | 8 | All 4 Types | 76% | Strong | Shows maximum possible strength for a very short string—perfect randomness is key here (zero deductions). |
| RedCarpetBlueShoes$1985 | 23 | Highly Mixed (Passphrase) | 100% | Very Strong | Optimal Passphrase Strategy: Length dominates the score, achieving perfect security despite minor pattern deductions. |
| qwertyuiop | 10 | Lowercase Only | 12% | Very Weak | Confirms that sequential keyboard patterns and restricted character sets are highly penalized, regardless of moderate length. |
| C0mplex-L3ngth-!23 | 16 | All 4 Types | 100% | Very Strong | Ideal Entropy: Perfect balance of significant length and maximum character set variety. |
| Z#q2t@R4&yB9^K5aG7 | 18 | All 4 Types | 100% | Very Strong | The most secure model: Long, perfectly complex, and fully avoids any sequence, repetition, or pattern deductions. |

III. Best Practices and Security Summary
Based on the quantitative results from the evaluation, the following best practices are identified for creating the strongest passwords.

Best Practices
1. Prioritize Length (Passphrases)
Tip Learned (Evidenced by Eg 7 & 9): A password should be 16 characters or longer. This is the single biggest factor affecting security. The jump in strength from 9 characters (Eg 4) to 16+ (Eg 9, 10) is exponential, moving the estimated time-to-crack from decades to millions of years.

Best Practice: Adopt a passphrase strategy (e.g., four random, unrelated words) to achieve high length while remaining memorable.

2. Maximize Character Set Variety
Tip Learned (Evidenced by Eg 2 vs. Eg 1): Mixing at least three character types (Uppercase, Lowercase, Numbers, Symbols) is mandatory. The difference between Eg 1 (single type) and Eg 2 (three types), both at 6 characters, was a +32 percentage point increase in score.

Best Practice: Always use a random mix of all four types, especially symbols and numbers placed in the middle, to maximize the character set (entropy).

3. Eliminate All Patterns
Tip Learned (Evidenced by Eg 3, 5, 8): Deductions for Consecutive Characters (e.g., aaaa or 111) and Sequential Characters (e.g., abcd) are severe. These patterns dropped the score of the 12-character password (Eg 3) by over 10 points.

Best Practice: Ensure no letters or numbers appear in sequence. Random generation (as in Eg 10) is the only way to perfectly eliminate these patterns.

IV. Research Summary: Common Password Attacks
Brute Force Attack: This attack attempts every single possible combination of characters, numbers, and symbols until the correct password is found. Security Defense: Length is the only effective defense, as it exponentially increases the time required for the attacker to search the entire keyspace.

Dictionary Attack: This is a focused attack that uses a pre-compiled list (a dictionary) of common words, phrases, and leaked credentials to test against hashes. Security Defense: Avoiding dictionary words and simple substitutions (like using l33t speak) is the primary defense.

V. Summary: How Password Complexity Affects Security
Password complexity affects security by increasing entropy (the unpredictability of the password).

Complexity Increases the Keyspace (Linear Gain): By adding symbols and numbers, you increase the number of possible characters an attacker must guess (e.g., from 52 letters to 95 characters). This provides a linear increase in security.

Length Provides Exponential Security (Dominant Gain): Length is the dominant factor because it raises the keyspace to an exponential power. For example, moving from an 8-character password to a 16-character password is not twice as secure—it is millions of times more secure.

The Conclusion: A secure password must be long and random. Complexity helps, but if a password is short, a highly complex character set is quickly defeated.

Password Security Analysis
1. What makes a password strong?
A strong password possesses high entropy, which is achieved by maximizing two components: length and character set variety.

Evidence from Table: The ideal password, Eg 10 (18 characters, All 4 types, 100% Score), achieved its perfect score because it combined long length with every available character set (uppercase, lowercase, numbers, and symbols) while eliminating all internal patterns. This combination makes it computationally infeasible for attackers to guess.

2. What are common password attacks?
The two most common password attacks are:

Brute Force Attack: This attempts every single possible character combination until the correct password is found. It is limited only by computing power and is defended primarily by password length.

Dictionary Attack: This is a more efficient, focused attack that uses lists of common words, famous names, and leaked credentials. It is designed to quickly crack passwords that rely on human memorability.

Evidence from Table: Passwords like Eg 3 (a common phrase/pattern, 50% score) and Eg 5 (a long but recognizable phrase, 26% score) are highly vulnerable to dictionary and pattern-based attacks because they fail to achieve true randomness.

3. Why is password length important?
Password length is the most critical factor because it increases the time required for a brute-force attack exponentially.

Evidence from Table:

A short password with mixed types, like Eg 2 (6 characters, 38%), offers minimal security (often seconds/minutes to crack).

A long, high-entropy password like Eg 9 (16 characters, 100%) moves the estimated time-to-crack to millions of years. The difference between a 9-character password (Eg 4) and a 16-character password (Eg 9) is exponential, proving that length is the dominant security defense.

4. What is a dictionary attack?
A dictionary attack is an attempt to crack a password by testing it against a pre-compiled list of common words, phrases, and simple variations (e.g., adding "123" or capitalizing the first letter).

Evidence from Table: The severe penalties applied to passwords containing sequential characters (Eg 3) or single character sets (Eg 5) are designed to simulate the success of a dictionary attack. The checker's Letters Only deduction, seen in Eg 5 (-25 points), is a direct countermeasure against this type of attack, flagging the password as weak regardless of its 25-character length.

5. What is multi-factor authentication (MFA)?
MFA is an authentication method that requires a user to provide two or more verification factors from different categories to gain access. These categories are typically:

Knowledge (something you know, like a password).

Possession (something you have, like a phone/token).

Inheritance (something you are, like a fingerprint).

MFA provides the essential security layer needed when a password, no matter how strong, is compromised via a breach or phishing attack.

6. How do password managers help?
Password managers are essential tools that solve the two biggest password security problems: memorability and reuse. They assist by:

Generating High-Entropy Passwords: They create the perfectly random, long, and complex strings that are difficult for humans to invent.

Evidence from Table: They generate passwords exactly like Eg 10—long, complex, and guaranteed to have zero sequential or repetitive deductions.

Enforcing Uniqueness: They store a unique password for every single service, mitigating the risk of credential stuffing after one site is breached.

7. What are passphrases?
Passphrases are long sequences of random, often unrelated words (e.g., correct-horse-battery-staple). They are considered a best practice because they are highly secure while being relatively easy for a human to remember.

Evidence from Table: Eg 7 (RedCarpetBlueShoes$1985, 23 characters, 100%) is a perfect example. This strategy provides the dominant security benefit of extreme length while remaining memorable enough to type.

8. What are common mistakes in password creation?
The most common mistakes are those that introduce predictable patterns that an attacker can easily guess or automate:

Using Sequential Patterns: Using characters in order on the keyboard or numerically.

Evidence from Table: Eg 8 (qwertyuiop, 12%) clearly shows the failure of this approach, as the highly predictable pattern is penalized and results in a "Very Weak" score.

Using Only One Character Type: Failing to mix uppercase, lowercase, numbers, and symbols.

Password Reuse: Using the same password across multiple sites, making every account vulnerable once the password is leaked from just one breach.
