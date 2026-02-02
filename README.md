graph TD
    %% --- STYLE DEFINITIONS ---
    classDef hub fill:#2A2A2A,stroke:#D4AF37,stroke-width:3px,color:#fff;
    classDef academy fill:#6A0DAD,stroke:#fff,stroke-width:2px,color:#fff;
    classDef equity fill:#0056D2,stroke:#fff,stroke-width:2px,color:#fff;
    classDef elig fill:#104E8B,stroke:#fff,stroke-width:2px,color:#fff;
    classDef bridge fill:#fff,stroke:#D4AF37,stroke-width:2px,stroke-dasharray: 5 5;

    %% --- ROOT: The Consortium Governance ---
    Consortium[("The MEA Consortium<br/>(Unified Governance Board)")]:::hub
    
    %% --- THE STRATEGIC BRIDGE (MEA GAMES) ---
    %% Described as the "Shim" or "Funnel" connecting the loops [cite: 398, 651]
    Games(MEA Games<br/>'Play with Purpose'<br/>The Engagement Bridge):::bridge
    Consortium --> Games

    %% --- ORG 1: META ETHICS ACADEMY (The Mind) ---
    %% Focus: Social & Moral Engineering [cite: 396, 497]
    subgraph MEA_1 [MEA: Meta Ethics Academy]
        direction TB
        Ac_Root[<b>Meta Ethics Academy</b><br/><i>'Engineering the Framework'</i>]:::academy
        Ac_Dept1[Dept: R&D<br/>(Moral Simulations)]:::academy
        Ac_Dept2[Dept: Education<br/>(Ethical Leadership)]:::academy
        
        Ac_Root --> Ac_Dept1
        Ac_Root --> Ac_Dept2
    end

    %% --- ORG 2: MISSION EQUITY ALLIANCE (The Heart) ---
    %% Focus: Second Chance & Systemic Resources [cite: 396, 619]
    subgraph MEA_2 [MEA: Mission Equity Alliance]
        direction TB
        Eq_Root[<b>Mission Equity Alliance</b><br/><i>'Systemic Equity & Resources'</i>]:::equity
        Eq_Dept1[Dept: Transition<br/>(Veteran Integration)]:::equity
        Eq_Dept2[Dept: Advocacy<br/>(Resource Allocation)]:::equity
        
        Eq_Root --> Eq_Dept1
        Eq_Root --> Eq_Dept2
    end

    %% --- ORG 3: MILITARY ELIGIBILITY ALLIANCE (The Hands) ---
    %% Focus: Administrative Access & Waiver Warriors [cite: 570, 608]
    subgraph MEA_3 [MEA: Military Eligibility Alliance]
        direction TB
        El_Root[<b>Military Eligibility Alliance</b><br/><i>'The Administrative Bridge'</i>]:::elig
        El_Dept1[Dept: Access<br/>(Waiver Processing)]:::elig
        El_Dept2[Dept: Recruitment<br/>(Fitness & Standards)]:::elig
        
        El_Root --> El_Dept1
        El_Root --> El_Dept2
    end

    %% --- CONNECTIONS & FLOW ---
    %% The Consortium governs all three
    Consortium --> Ac_Root
    Consortium --> Eq_Root
    Consortium --> El_Root

    %% The Bridge (Games) feeds all three [cite: 401, 663]
    Games -.->|Identifies Leaders| Ac_Root
    Games -.->|Directs Resources| Eq_Root
    Games -.->|Recruits Talent| El_Root

    %% Synergies defined in the "Ecosystem" [cite: 396]
    Ac_Dept1 --"Ethical Design"--> Games
    Eq_Dept1 --"Beneficiaries"--> El_Dept1
