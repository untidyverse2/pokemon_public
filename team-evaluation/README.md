**Team-Evaluation** Module:

This folder contains scripts and data related to evaluating Pokémon teams in the context of competitive gameplay in an attempt to translate concepts and heuristics around into code and automate a data-driven approach. 
The evaluation process involves analyzing team compositions, scoring stats combinations, roles, types, threat coverage, and weaknesses against common threats. 
The goal is to find a heuristic approach to evaluate Pokémon teams that excel in multiple competitive scenarios according to the different criterias suggested by Pokémon experts.


Key Features:

**Team Evaluation**: Combination of scoring metrics for: role diversity, type uniqueness, stats evaluation, threat converage and weaknesses in order to be able to rank "best team" combinations.
evaluate_team_combinations.R: Main script that evaluates team combinations based on automated criteria and weights to identify the best possible team.

- Role Classification and Scoring: Classifies Pokémon into roles such as Physical Attacker, Special Attacker, Defensive Wall, Support, etc.
score_role_diversity.R: Function that scores the diversity in the roles.

- Type Uniqueness Scoring: Logic to score the diversity of types within the team, also considering redundancies.
score_type_uniqueness.R: Function that scores type diversity within the team, penalizing redundant types.

- Stats Evaluation: 
calculate_max_level_stats.R: Function that uses a combined approach to calculate a comprehensive stats summary for each pokémon that reflects multiple aspects.

- Weakness Analysis: Evaluates team weaknesses against different threats relaetd to their move effectiveness and type coverage.
evaluate_team_weaknesses.R: Function that checks team weaknesses by analyzing the move types of each pokemon.

- Threat Coverage Scoring: Logic to score common threats focused on get collective team synergy.
score_coverage_against_threats.R: Function that scores team coverage against threats. 
