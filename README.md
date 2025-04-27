# AA_Tournament
# Strategy

The Tenfold Wrath strategy is a calm yet firm approach to the Iterated Prisoner's Dilemma. It begins with full cooperation and remains cooperative even when the opponent defects once. However, after the second defection, it switches to a retaliation phase, during which it defects for 10 consecutive rounds to punish repeated betrayal.

Once these 10 rounds are completed, the strategy evaluates the opponent's behavior. If the opponent returns to cooperating, Tenfold Wrath also resumes cooperation, giving them a chance to rebuild trust. If the opponent continues to defect, the strategy will keep defecting until cooperation is observed again.

This cycle repeats throughout the game: cooperate until betrayed twice, then defect 10 times, reassess, and reset if cooperation returns.

The design of Tenfold Wrath promotes long-term cooperation while deterring repeated exploitation. It is forgiving but not naive, giving second chances but ensuring that betrayal comes with consequences. Its ability to reset and adapt makes it resilient against both random mistakes and malicious strategies.

In essence, Tenfold Wrath is a strategy built on patience, fairness, and intelligent retaliation—encouraging peace, but never tolerating prolonged hostility.

# Opponent Selection
The strategy also evaluates which opponents to interact with based on their cooperation history. It excludes any opponent with whom it has already played the maximum allowed rounds (200) and prioritizes those who exhibit a high level of cooperation. When choosing the next opponent, Tenfold Wrath selects from eligible candidates who have defected less frequently, aiming to maximize the chances of a cooperative environment. This ensures that the strategy doesn’t repeatedly engage in conflict with adversaries who are less likely to cooperate, preserving both the integrity of the game and its long-term goals.