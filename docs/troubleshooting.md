# Troubleshooting and Lessons

## The main problem

After the initial WireGuard deployment, the original VPS IP became unreliable for the intended connections. The service itself deployed correctly, so the issue was in connectivity rather than configuration.

**What I did:** researched possible network restrictions and alternative approaches (including Chinese-language technical forums), obtained a replacement IP, and tried other stacks.

**What I did not establish:** the precise cause. I treat it as an observed connectivity/accessibility problem, not a confirmed case of a specific restriction.

## Lessons

- A service can deploy successfully and still be unreliable on a particular network path.
- IP accessibility and network filtering can affect self-hosted services.
- Testing from several client devices gives a more realistic view of compatibility than testing from one.
- 1 CPU core and 1 GB RAM constrain service choice and should be considered up front.
- Trying several implementations and researching alternatives is a practical way to work through infrastructure problems.
