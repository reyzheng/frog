# frog
statitcs of frog MBA sign-ups

## Commands
-f: input file name__
-c: command__
__
subcommands:__
    1. name: print the sign-up counts and years of specified member__
        sample: python .\frog\frog.py -f .\2020-2025.xlsx -c name:吳天心__
    2. cons: print members who sign-up continually till the specified year__
        sample: python .\frog\frog.py -f .\2020-2025.xlsx -c cons:2024,2__
        -> list duplicated members from 2023 to 2024__
        sample: python .\frog\frog.py -f .\2020-2025.xlsx -c cons:2024,3__
        -> list duplicated members from 2022 to 2024__
    3. conpercentage: list duplicated members of specified year and its previous__
        sample: python .\frog\frog.py -f .\2020-2025.xlsx -c conpercentage:2022__
        -> list duplicated members from 2021 to 2022 and calculate percentage (based on previous year)
