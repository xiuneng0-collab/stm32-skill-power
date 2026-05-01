# STM32 Skills Pack

A small Codex skill pack for common STM32 firmware work.

This pack is intentionally generic:

- no project-specific logic
- no board-specific assumptions
- no fixed chip model dependency
- focused on basic STM32 workflows that show up often in real projects

## Included Skills

### `stm32-project-thinking`

General STM32 working style.

Use it for:

- overall project analysis
- structured troubleshooting
- deciding what to check first
- avoiding premature complexity

### `stm32-debugging`

Focused fault isolation for STM32 runtime problems.

Use it for:

- startup failure
- hangs and deadlocks
- no output
- interrupt issues
- DMA issues
- unstable runtime behavior

### `stm32-pin-planning`

Focused pin-truth and mux-conflict checking.

Use it for:

- actual pin usage mapping
- alternate-function checks
- board-level pin conflicts
- code vs generated config mismatch

### `stm32-migration`

Focused project porting guidance.

Use it for:

- moving old firmware to a new board
- separating validated behavior from board adaptation
- preserving existing behavior during migration

### `stm32-peripheral-bringup`

Focused single-peripheral bring-up.

Use it for:

- GPIO
- UART
- SPI
- I2C
- ADC
- PWM
- timers
- simple DMA

## Directory Structure

Each skill follows the Codex skill layout:

```text
skill-name/
|-- SKILL.md
`-- agents/
    `-- openai.yaml
```

## Install

Copy the skill folders into your Codex skills directory, for example:

```text
~/.codex/skills/
```

or on Windows:

```text
C:\Users\<YourUser>\.codex\skills\
```

## Notes

- These skills are written for practical STM32 work, not for one specific SDK or board.
- They are designed to be simple, conservative, and easy to trigger.
- You can publish each skill separately or keep them together as one pack.
