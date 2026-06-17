# Lyceum — Claude Code plugin marketplace

This repository is a [Claude Code](https://code.claude.com) **plugin marketplace** that hosts **Lyceum**, a portable, evidence-based meta-learning system: nine coordinated skills that teach *any* subject from absolute beginner to mastery using the techniques with the strongest support in learning science (retrieval practice, spaced repetition, interleaving, deliberate practice, mastery learning, backward design).

## Install

In Claude Code:

```
/plugin marketplace add Patryk-beep/lyceum
/plugin install lyceum@lyceum-marketplace
```

Then restart the session — all nine skills become available as `lyceum:<skill>`.

## What's inside

```
.
├── .claude-plugin/marketplace.json   # marketplace manifest
└── plugins/lyceum/                   # the Lyceum plugin
    ├── .claude-plugin/plugin.json
    ├── README.md                     # full skill list + architecture
    ├── skills/                       # 9 skills (learn, research-topic, …, capstone)
    └── references/                   # 6 shared reference files
```

See [`plugins/lyceum/README.md`](plugins/lyceum/README.md) for the full skill list, how the chain works, and the "copy the `learning/<subject>/` folder = save file" portability model.

## Using it

Say what you want to learn — e.g. *"I want to learn the Roman Republic, get me to seminar level"* — and `lyceum:learn` sets up a workspace and routes you through research → curriculum → teach → assign → assess → review per module, gating each step on measured mastery, until a capstone certifies you. Ask **"what's next?"** any time to resume.

## License

MIT — see [LICENSE](LICENSE).
