# Aethrix

Aethrix is a suite of plugins for [openac-rust](https://github.com/eriknihlen/openac-rust), the Asheron's Call client written in Rust. It's designed to automate parts of play and to bring quality of life improvements, with each plugin doing one job and running on its own.

This repository holds the suite's releases. The source is private for now, and we intend to open-source it once the suite is feature complete.

## Aethrix Vision

Vision is the first plugin in the suite, and this is its first version, **0.1.0**.

Vision finds the objects and people you're watching for. You tell it what to look for with searches, by name, by kind, by object class or by a pattern, and it:

- marks each find in the world with a gem and a label showing its name and distance, in its search's colour;
- lists what it has found in its window, where you can select a find or ignore it;
- shows the nearest finds on a HUD, with an arrow pointing to each one, and a toast when something new appears;
- tells you in chat when a search finds something;
- can shade the ground you can't walk on, such as cliffs and open sea.

Open it with `/vision`, or `/av` for short. Every setting has a sensible default and can be changed in its settings window; the [wiki](https://github.com/davidc-smith/OpenAC-Aethrix/wiki) lists them all.

## Installing

Install Aethrix Vision from the openac-rust launcher's plugin list.

## Problems

If something goes wrong, Vision can write a problem report to send us with an issue.
