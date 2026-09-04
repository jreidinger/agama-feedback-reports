# Agama User Feedback Reports

This repository stores monthly user feedback reports and the AI instructions used to generate them for **Agama**, the new SLES/openSUSE web-based installer.

## Repository Structure

- **`reports/`**: Contains the generated monthly feedback reports (e.g., `2026-8.md`, `2026-9.md`). These reports synthesize positives, negatives, and suggestions for improvement from various community hubs, forums, and external sources.
- **`instructions/`**: Contains the instructions for AI agents to generate new reports. 
  - `FEEDBACK.md`: Detailed prompt and step-by-step instructions for searching, analyzing, and structuring the feedback report for a given timeframe.

## Generating a New Report

To generate a new report, provide an AI agent (like this one) with the instructions located in [`instructions/FEEDBACK.md`](instructions/FEEDBACK.md). The agent will search for feedback from the previous month across various channels (forums, Reddit, blogs), categorize it, and output a structured Markdown report that can then be saved into the `reports/` directory.

## License

Please refer to the [LICENSE](LICENSE) file for more information.
