# Bolinao Lexicon: Rule-Based Morphological Analysis

This repository contains a Jupyter Notebook, [`Bolinao_Lexicon_Processing.ipynb`], dedicated to the computational analysis of the Bolinao language. The project focuses on identifying and reversing various morphophonological processes to derive root words from their surface forms.

The methodology involves a rule-based approach where linguistic patterns are programmatically applied to a comprehensive Bolinao lexicon.

## Key Features

1.  **Web Scraping**: The notebook includes a scraper to collect lexical data from the Webonary Bolinao dictionary.
2.  **Data Preprocessing**: Extensive cleaning and preparation of the scraped data, including POS tagging normalization from Webonary standards to Universal POS tags.
3.  **Morphological Analysis**: Implementation of rule-based algorithms to identify and reverse several key linguistic phenomena in Bolinao.

## Morphophonological Processes Analyzed

The analysis covers the following processes, with scripts designed to find the root word for each case:

*   **Dissimilation**: Consonant changes (e.g., `p` → `k`, `b` → `g`) triggered by the `-um-` infix.
*   **Assimilation**: Sound changes where prefixes like `maN-`, `aN-`, and `saN-` adapt to the following consonant.
*   **Assimilation and Reduction**: A process where prefixes such as `maNg-` cause both assimilation and the deletion of the root's initial consonant.
*   **Gemination and Vowel Reduction**: Consonant doubling that occurs as a result of vowel loss (syncope).
*   **Number or Mass Indication**: Analysis of reduplication and infixation (e.g., `-aw-`, `-u-`) used to indicate quantity.
*   **Pronoun Alternations**: Morphophonemic changes in interrogative, indefinite, and demonstrative pronouns.
*   **Vowel Reduction**: Reversing the process where vowels are dropped between consonants.

## Methodology

For each linguistic process, the notebook follows a consistent workflow:
1.  Define the morphophonological rule based on linguistic descriptions.
2.  Implement a function to generate potential root word candidates by reversing the rule.
3.  Cross-validate the generated candidates against the cleaned Bolinao lexicon.
4.  Save the confirmed pairs (surface form and its root) to a `.csv` file for further analysis.

This project serves as a practical application of computational linguistics to a low-resource language, creating a foundation for a rule-based stemmer for Bolinao.