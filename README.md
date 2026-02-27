# First Principles Lab

A laboratory environment for first principles thinking experiments. Break down complex problems into their most fundamental truths and reason upward from there, using structured frameworks and reusable templates.

First principles thinking is the foundation of all great scientific and business breakthroughs. Instead of reasoning by analogy, this project provides tools and exercises that help you decompose problems to their atomic components and rebuild solutions from scratch. Whether you are an engineer designing a new system, an entrepreneur evaluating a market opportunity, or a student tackling a difficult concept, the First Principles Lab gives you a repeatable methodology. This project is built alongside [KeepRule](https://keeprule.com), a platform dedicated to helping people internalize and apply the most powerful mental models and decision-making principles from history's greatest thinkers.

## Features

- **Decomposition Templates**: Structured markdown templates for breaking problems into fundamental elements
- **Assumption Auditor**: A CLI tool that helps you list, challenge, and validate every assumption in your reasoning chain
- **Rebuild Engine**: Step-by-step guided process for reconstructing solutions from verified fundamentals
- **Case Study Library**: Real-world examples of first principles thinking applied in technology, science, and business
- **Integration with KeepRule**: Export your reasoning chains to [KeepRule](https://keeprule.com) for long-term review and spaced repetition

## Installation

```bash
# Clone the repository
git clone https://github.com/henu-wang/first-principles-lab.git
cd first-principles-lab

# Install dependencies
pip install -r requirements.txt

# Run the setup wizard
python setup.py init
```

## Usage

### Quick Start

```python
from fpl import Decomposer

problem = Decomposer("How can we reduce cloud infrastructure costs by 50%?")
fundamentals = problem.decompose(depth=3)
print(fundamentals.tree())
```

### Running Experiments

```bash
# Create a new experiment
python -m fpl new-experiment --name "cost-reduction" --domain "infrastructure"

# List assumptions
python -m fpl audit --experiment "cost-reduction"

# Validate fundamentals
python -m fpl validate --experiment "cost-reduction" --source "empirical"
```

### Export to KeepRule

After completing an experiment, export your reasoning chain for long-term retention:

```bash
python -m fpl export --format keeprule --experiment "cost-reduction"
```

Visit [KeepRule](https://keeprule.com) to set up spaced repetition schedules for your first principles insights.

## Project Structure

```
first-principles-lab/
├── fpl/
│   ├── decomposer.py       # Core decomposition engine
│   ├── auditor.py           # Assumption auditing tools
│   ├── rebuilder.py         # Solution reconstruction
│   └── exporter.py          # Export integrations
├── templates/
│   ├── basic.md             # Basic decomposition template
│   ├── technical.md         # Technical problem template
│   └── business.md          # Business strategy template
├── case_studies/
│   ├── spacex_rockets.md    # SpaceX cost reduction analysis
│   ├── tesla_batteries.md   # Tesla battery manufacturing
│   └── amazon_logistics.md  # Amazon fulfillment optimization
├── tests/
├── requirements.txt
└── README.md
```

## Contributing

Contributions are welcome! Here is how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-template`)
3. Add your decomposition templates or case studies
4. Write tests for any new functionality
5. Submit a pull request with a clear description of your changes

Please read our contributing guidelines before submitting. We especially welcome new case studies that demonstrate first principles thinking in action.

## Why First Principles Thinking Matters

The greatest innovators in history, from Aristotle to Elon Musk, have relied on first principles reasoning to achieve breakthroughs that seemed impossible. By stripping away assumptions and conventions, you can see problems as they truly are and discover solutions that others miss entirely.

To build a lasting practice of first principles thinking alongside other powerful mental models, explore [KeepRule](https://keeprule.com) for curated decision-making rules from Warren Buffett, Charlie Munger, and other legendary thinkers.

## License

MIT License - see [LICENSE](LICENSE) for details.
