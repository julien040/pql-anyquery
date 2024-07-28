# pipelined query language

[![Website](https://img.shields.io/badge/INTRO-WEB-blue?style=for-the-badge)](https://pql.dev)
[![Playground](https://img.shields.io/badge/INTRO-PLAYGROUND-blue?style=for-the-badge)](https://pql.dev)
[![Discord](https://img.shields.io/discord/1120882187785470113?label=discord%20chat&style=for-the-badge)](https://discord.gg/PbeXzrWP)

This is a simple fork of PQL repository to suit the needs of [Anyquery](https://anyquery.dev) project.

## Changes

- EQ operator does not use the coalesce function anymore. This change was needed because if a table parameter was used, SQLite wouldn't return the constraint to the vtable because PQL would embrace it with a coalesce function.
