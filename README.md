# Chess Data Exploration

## Objectives

This project aims to perform exploratory data analysis and preprocessing on chess match data. Using the provided dataset, the goal is to analyse:

- Win distribution based on the colors (white vs. black).
- Which chess openings result in more victories for each color.
- The influence of player rating on the likelihood of winning or drawing.
- Draw tendencies for specific openings.
- Identification of potential outliers in player ratings and their impact on the analysis.

The analyses focus on understanding the relationship between chess openings, player ratings, and match outcomes.

## Dataset

The dataset used in this project, **games.csv** file on this repository, contains detailed information about chess matches, and is also available on Kaggle: [Link](https://www.kaggle.com/datasets/datasnaek/chess).

### Dataset Column Descriptions

| Column Name       | Description                                                      |
|-------------------|------------------------------------------------------------------|
| turns             | Total number of moves made in the match.                        |
| victory_status    | Status of the match's victory (“mate”, “resign”, “timeout”, “draw”).|
| winner            | Player who won the match ("white", "black", or "draw").        |
| white_rating      | Rating of the player playing with white pieces.                 |
| black_rating      | Rating of the player playing with black pieces.                 |
| opening_name      | Name of the opening played.                       |
| opening_ec        | ECO code related to the opening played.                         |
| opening_ply       | Depth of the opening in number of moves.                        |

*ECO code can be found [here](https://www.365chess.com/eco.php).*

**Note:** The following columns from the original dataset were not utilized in this analysis:  
- id, rated, created_at, last_move_at, increment_code, white_id and black_id

### Categorical variables

- winner: Categorical, with values such as “white”, “black”, “draw”.
- opening_name: Categorical, representing the name of the opening used in the match.
- victory_status: Categorical, with values such as “mate”, “resign”, “timeout”, “draw”.

### Numeric variables

- white_rating: Numeric, representing the rating of the player who played white.
- black_rating: Numeric, representing the rating of the player who played black.
- turns: Numeric, representing the number of moves in the match.

## Code

All the code used for the analyses can be accessed in the Google Colab notebook: [Link](https://colab.research.google.com/drive/1cNCWm20XncsTvTy0aamZq5W0HVh_4p6T?usp=sharing)
