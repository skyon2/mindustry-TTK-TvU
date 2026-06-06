# Mindustry Turret vs Unit TTK benchmark

Hello! I'm Skyon.

This spreadsheet contains Time-to-Kill (TTK) benchmark data for Mindustry turrets against units.

**Important:** These values are **survival time (seconds)**, not DPS.

## Methodology

1. All tests are performed using World Processors.
2. Turret distance is:
   - 4 blocks for 1v1 tests
   - 10 blocks for 5v5 tests
   - Unless otherwise noted (for example, "5 dis").
3. Before a test begins, an invincible unit is spawned to warm up the turret and allow it to acquire a target after cooldown.
4. As soon as the actual test unit spawns, the turret starts firing and the timer starts.
5. Units remain in the center of the test area. In group tests, the final surviving unit receives knockback resistance.
6. The timer stops once all units of the same type are destroyed.
7. If a unit survives longer than 120 seconds, logic predicts the estimated kill time and marks the result with `≈`.
8. If a turret cannot damage a unit (for example, Titan vs Avert), the result is marked as `N`.
9. If a unit still has nearly full HP after the 120-second timeout, the result is marked as `≈MaxHp`.
10. If the predicted kill time exceeds 10,000 seconds, the result is marked as `≈T`.
11. **Serpulo only:** For average calculations:
    - `≈T` and `≈MaxHp` are treated as 10,000 seconds.
    - `N` values are ignored.
12. **Serpulo only:** In 1v1 tests, status effects are applied using Tsunami. In 5v5 tests, World Processors apply the status effect directly to all units, unless a specific turret setup is noted (for example, "5 wave").
13. **nfb** means **No Fire-rate Boost**:
    - No Overdrive Projector
    - No liquid fire-rate boost
    - Unless required for the turret's operation (such as Meltdown).

## Known Issues

- Timing may be slightly inaccurate (for example, ±0.5s, ±1s, etc.).
- Turret reaction time, aiming behavior, and accuracy can affect results.
- If an air unit is falling but still alive, the timer does not stop until the unit reaches the ground.
- Prediction logic is not perfectly accurate, especially for slow-firing turrets such as Scathe.
- **Serpulo only:** Oil Tsunami/status combinations are not included because the number of Oil Tsunamis significantly affects the results.
