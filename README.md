# frog
statitcs of frog MBA sign-ups

## Commands
- -f: input file name
- -c: command
  - subcommands:
    - name: print the sign-up counts and years of specified member
      - sample: python .\frog\frog.py -f .\2020-2025.xlsx -c name:吳天心
    - cons: print members who sign-up continually till the specified year
      - sample: python .\frog\frog.py -f .\2020-2025.xlsx -c cons:2024,2
        -> list duplicated members from 2023 to 2024
      - sample: python .\frog\frog.py -f .\2020-2025.xlsx -c cons:2024,3
        -> list duplicated members from 2022 to 2024
    - conpercentage: list duplicated members of specified year and its previous
      - sample: python .\frog\frog.py -f .\2020-2025.xlsx -c conpercentage:2022
        -> list duplicated members from 2021 to 2022 and calculate percentage (based on previous year)
