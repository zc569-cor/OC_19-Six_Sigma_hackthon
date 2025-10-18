# The Quality Control System of NY solar power plants
This repo is for the Hackthon project
```mermaid
flowchart TD
    %% Inputs
    A1[Weather condition<br>(input)] -->|Mapping| B[Theoretical Power]
    A2[Date<br>(input)] -->|Attenuate to (%)| B
    A3[Actual Power<br>(input)] --> C[(Rate = Ac / The)]
    
    %% Computation Flow
    B --> C
    C --> D[Health Rate %]
    D --> E[Input CPK]
    E --> F[Find and pop an error]



