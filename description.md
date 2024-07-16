# Bases
### Write in editor:
`base`
### Description
This snippets writes out all the base robot files so you can use the bot templates.
### Prints
```
#base robot_giant.pop
#base robot_standard.pop
#base robot_gatebot.pop
```

# Wave Schedule with 3 Waves
### Write in editor:
`ws3`
### Description
This snippets prints out a WaveSchedule with 3 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-3 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 3
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with 4 Waves
### Write in editor:
`ws4`
### Description
This snippets prints out a WaveSchedule with 4 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-4 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 4
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 4 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave4a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with 5 Waves
### Write in editor:
`ws5`
### Description
This snippets prints out a WaveSchedule with 5 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-5 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 5
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 4 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave4a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 5 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave5a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with 6 Waves
### Write in editor:
`ws6`
### Description
This snippets prints out a WaveSchedule with 6 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-6 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 6
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 4 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave4a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 5 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave5a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 6 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave6a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with 7 Waves
### Write in editor:
`ws7`
### Description
This snippets prints out a WaveSchedule with 7 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-7 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 7
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 4 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave4a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 5 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave5a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 6 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave6a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 7 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave7a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with 8 Waves
### Write in editor:
`ws8`
### Description
This snippets prints out a WaveSchedule with 8 waves filled automatically so you can immediately start writing WaveSpawns.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-8 Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 8
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave1a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 2 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave2a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 3 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave3a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 4 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave4a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 5 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave5a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 6 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave6a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 7 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave7a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }

    // Wave 8 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay // Replace with "Target wave_start_relay_classic" for Rottenburg
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

        // Subwave description here
        WaveSpawn
        {
            Name "wave8a"
            Where spawnbot
            TotalCount 12
            MaxActive 6
            SpawnCount 3
            WaitBeforeStarting 0
            WaitBetweenSpawns 10
            TotalCurrency 60
            TFBot
            {
                Class Scout
                Skill Hard
            }
        }
    }
}
```
# Wave Schedule with no WaveSpawns
### Write in editor:
`wsnw`
### Description
This snippets prints out a WaveSchedule with no WaveSpawns and only 1 wave.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line

    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
    // Wave 1-X Sentry Busters
    Mission
    {
        Objective           DestroySentries
        Where               spawnbot
        BeginAtWave         1
        RunForThisManyWaves 5
        CooldownTime        70
        DesiredCount        1
        InitialCooldown     30
        TFBot
        {
            Template T_TFBot_SentryBuster
        }
    }

    // Wave 1 - X Currency
    Wave
    {

        StartWaveOutput
        {
            Target wave_start_relay
            Action Trigger
        }

        DoneOutput
        {
            Target wave_finished_relay
            Action Trigger
        }

    }
}
```
# Wave Schedule with Only KeyValues
### Write in editor:
`wskv`
### Description
This snippets prints out a WaveSchedule with only the KeyValues filled out. This could be useful for robot/wavespawn template popfiles.
### Prints
```
WaveSchedule
{
    StartingCurrency                      400
    RespawnWaveTime                       7
    FixedRespawnWaveTime                  No
    CanBotsAttackWhileInSpawnRoom         No
    AddSentryBusterWhenKillCountExceeds   15
    AddSentryBusterWhenDamageDealtExceeds 3000
    Advanced                              0 // Only enable for Advanced/Expert/higher missions (for achievements)
    EventPopFile                          Halloween // If you don't want this mission to be like wave 666 then delete this line
    IsEndless                             0 // Activate super secret endless MvM mode (i dont know what this is)
}
```
# Sniper Mission
### Write in editor:
`msnip`
### Description
This snippets prints out a Sniper support Mission with everything easily available to change.
### Prints
```
// Wave X Snipers
Mission
{
    Objective           Sniper
    Where               spawnbot_mission_sniper
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        20
    DesiredCount        5
    InitialCooldown     10
    TFBot
    {
        Template T_TFBot_Sniper
    }
}
```
# Spy Mission
### Write in editor:
`mspy`
### Description
This snippets prints out a Spy support Mission with everything easily available to change.
### Prints
```
// Wave X Spies
Mission
{
    Objective           Spy
    Where               spawnbot_mission_spy
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        60
    DesiredCount        2
    InitialCooldown     10
    TFBot
    {
        Template T_TFBot_Spy
    }
}
```
# Sentry Buster Mission
### Write in editor:
`mds` or `msb`
### Description
This snippets prints out a Sentry Buster support Mission with everything easily available to change.
### Prints
```
// Wave X Sentry Busters
Mission
{
    Objective           DestroySentries
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        80
    DesiredCount        1
    InitialCooldown     20
    TFBot
    {
        Template T_TFBot_SentryBuster
    }
}
```
# Engineer Mission
### Write in editor:
`meng`
### Description
This snippets prints out a Engineer support Mission with everything easily available to change.

This is a snippet for the 'Engineer Sentry Teleporter' template meaning that it has 500 HP, teleports into the map, and build a sentry gun and teleporter.
### Prints
```
// Wave X Teleporter Engis (Teleports into map (does not spawn at spawnbot) and tries to build sentry and tele)
Mission
{
    Objective           Engineer
    InitialCooldown     40
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        30
    DesiredCount        1

    TFBot
    {
        Template T_TFBot_Engineer_Sentry_Teleporter
    }
}
```
# Battle Engineer Mission
### Write in editor:
`mbeng`
### Description
This snippets prints out a Battle Engineer support Mission with everything easily available to change.

This is a snippet for the 'Engineer Sentry Tele Battle' template meaning that it has 275 HP, __does not__ teleport into the map (it spawns with the rest of the bots), and builds a sentry gun and teleporter.
### Prints
```
// Wave X Battle Teleporter Engis (Does not teleport into map (spawns at spawnbot) and tries to build sentry and tele)
Mission
{
    Objective           Engineer
    InitialCooldown     40
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        30
    DesiredCount        1

    TFBot
    {
        Template T_TFBot_Engineer_Sentry_Tele_Battle
    }
}
```
# Sentry Engineer Mission
### Write in editor:
`mseng`
### Description
This snippets prints out a Sentry Engineer support Mission with everything easily available to change.

This is a snippet for the 'Engineer Sentry Battle TeleIn' template meaning that it has 275 HP, __teleports__ into the map, and builds **only a sentry gun**.
### Prints
```
// Wave X Sentry Engis (Teleport into map (does not spawn at spawnbot) and tries to build sentry, but will not build tele)
Mission
{
    Objective           Engineer
    InitialCooldown     40
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        30
    DesiredCount        1

    TFBot
    {
        Template T_TFBot_Engineer_Sentry_Battle_TeleIn
    }
}
```
# Sentry Battle Engineer Mission
### Write in editor:
`mseng`
### Description
This snippets prints out a Sentry Battle Engineer support Mission with everything easily available to change.

This is a snippet for the 'Engineer Sentry Battle TeleIn' template meaning that it has 275 HP, __does not__ teleport into the map (it spawns with the rest of the bots), and builds **only a sentry gun**.
### Prints
```
// Wave X Sentry Battle Engis (Does not teleport into map (spawns at spawnbot) and tries to build sentry, but will not build tele)
Mission
{
    Objective           Engineer
    InitialCooldown     40
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        30
    DesiredCount        1

    TFBot
    {
        Template T_TFBot_Engineer_Sentry_Battle
    }
}
```
# Blank Mission
### Write in editor:
`mblank`
### Description
This snippets prints out a blank Mission template so you can create your own Mission template.
### Prints
```
// Wave X [Botname]
Mission
{
    Objective           [Bot Type]
    InitialCooldown     40
    Where               spawnbot
    BeginAtWave         1
    RunForThisManyWaves 1
    CooldownTime        30
    DesiredCount        1

    TFBot
    {
        // Stuff goes here
    }
}
```
# Basic WaveSpawn Template
### Write in editor:
`wspb`
### Description
This snippets prints out a basic WaveSpawn template to ease creation of single-robot-type subwaves.
### Prints
```
// Subwave description here
WaveSpawn
{
    Name "waveXXy"
    Where spawnbot
    TotalCount 3
    MaxActive 3
    SpawnCount 3
    WaitForAllSpawned "waveXXy"
    WaitForAllDead "waveXXy" // You can only have either WFASpawned or WFADead
    WaitBeforeStarting 30
    WaitBetweenSpawns 15
    TotalCurrency 120
    Support Limited // This will make the robots appear in Support. 1 makes them spawn infinitely and Limited makes only TotalCount spawn. Delete this line to make them normal bots
    TFBot
    {
        // Put stuff here
    }
}
```
# Squad WaveSpawn Template
### Write in editor:
`wsps`
### Description
This snippets prints out a basic WaveSpawn template to ease creation of squad-type subwaves.
### Prints
```
// Subwave description here
WaveSpawn
{
    Name "waveXXy"
    Where spawnbot
    TotalCount 6
    MaxActive 2
    SpawnCount 2
    WaitForAllSpawned "waveXXy"
    WaitForAllDead "waveXXy" // You can only have either WaitForAllSpawned or WaitForAllDead
    WaitBeforeStarting 30
    WaitBetweenSpawns 15
    TotalCurrency 120
    Support Limited // This will make the robots appear in Support. 1 makes them spawn infinitely and Limited makes only TotalCount spawn. Delete this line to make them normal bots
    Squad
    {
        FormationSize 200
        ShouldPreserveSquad 1 // If the squad leader dies, should the rest stay as a squad
        TFBot
        {
            // Put stuff here
        }

        TFBot
        {
            // Put stuff here
        }
    }
}
```
# RandomChoice WaveSpawn Template
### Write in editor:
`wsprc`
### Description
This snippets prints out a basic WaveSpawn template to ease creation of random-choice subwaves.
### Prints
```
// Subwave description here
WaveSpawn
{
    Name "waveXXy"
    Where spawnbot
    TotalCount 6
    MaxActive 2
    SpawnCount 2
    WaitForAllSpawned "waveXXy"
    WaitForAllDead "waveXXy" // You can only have either WaitForAllSpawned or WaitForAllDead
    WaitBeforeStarting 30
    WaitBetweenSpawns 15
    TotalCurrency 120
    Support Limited // This will make the robots appear in Support. 1 makes them spawn infinitely and Limited makes only TotalCount spawn. Delete this line to make them normal bots
    RandomChoice
    {
        TFBot
        {
            // Put stuff here
        }

        TFBot
        {
            // Put stuff here
        }
    }
}
```
# Tank WaveSpawn Template
### Write in editor:
`wspt`
### Description
This snippets prints out a Tank WaveSpawn Template to make the creation of Tank subwaves easier.
### Prints
```
// X Tank(s)
WaveSpawn
{
    Name "waveXXy"
    TotalCount 1
    WaitForAllSpawned "waveXXy"
    WaitForAllDead "waveXXy" // You can only have either WaitForAllSpawned or WaitForAllDead
    WaitBeforeStarting 30
    WaitBetweenSpawns 15 // Only keep this if there will be more than one tank in this wavespawn
    TotalCurrency 400
    Tank
    {
        Name "tank01"
        Health 40000
        Speed 75
        StartingPathTrackNode "track_node"
        Skin 1
        OnKilledOutput
        {
            Target boss_dead_relay
            Action Trigger
        }

        OnBombDroppedOutput
        {
            Target boss_deploy_relay
            Action Trigger
        }
    }
}
```