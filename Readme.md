🚗🔐 𝑨𝒖𝒕𝒐𝒎𝒐𝒕𝒊𝒗𝒆 𝑪𝒚𝒃𝒆𝒓𝒔𝒆𝒄𝒖𝒓𝒊𝒕𝒚 𝑬𝒙𝒑𝒍𝒂𝒊𝒏𝒆𝒅: 𝑯𝒐𝒘 𝑬𝒏𝒈𝒊𝒏𝒆𝒆𝒓𝒔 𝑪𝒂𝒍𝒄𝒖𝒍𝒂𝒕𝒆 𝑹𝒊𝒔𝒌 𝑼𝒔𝒊𝒏𝒈 𝑰𝑺𝑶/𝑺𝑨𝑬 21434 (𝑻𝑨𝑹𝑨)
🚗🔒 When implementing cybersecurity in automotive systems, one of the most important steps is quantifying risk before implementing any protection mechanisms. This structured process is defined in ISO/SAE 21434 under Threat Analysis and Risk Assessment (TARA).
Below is a simplified explanation of how a risk value is calculated, using a practical example that beginners and engineers can both understand.
________________________________________
1️⃣ Identify the Asset 🚗
The first step is identifying the asset that needs protection.
Example asset:
Torque Request CAN Signal
This signal is critical because it directly influences vehicle acceleration and power delivery. If manipulated, it can directly affect vehicle safety and control.
📘 Reference Document:
ISO/SAE 21434 – Clause 15 (Threat Analysis and Risk Assessment) describes the identification of assets and the context for cybersecurity analysis.
🖼 Suggested Visual for Post
(Image idea: Vehicle architecture diagram highlighting CAN network and Torque signal)
________________________________________
2️⃣ Identify the Threat Scenario 🧑‍💻
Next, we define a realistic threat scenario.
Example threat:
An attacker injects or modifies a CAN message to manipulate the torque request value.
This could be performed using a CAN interface tool connected to the vehicle network, allowing malicious messages to be transmitted.
📘 Reference Document:
ISO/SAE 21434 – Clause 15.4 (Threat Scenario Identification) explains how to define possible attack scenarios affecting identified assets.
🖼 Suggested Visual for Post
(Image idea: CAN bus diagram showing attacker injecting a malicious message)
________________________________________
3️⃣ Impact Analysis ⚠️
ISO 21434 requires evaluating the impact of a successful attack across four categories:
• Safety Impact (S) – Could this endanger passengers or drivers?
• Financial Impact (F) – Could it cause financial loss to the OEM or customer?
• Operational Impact (O) – Could vehicle functionality be disrupted?
• Privacy Impact (P) – Could personal data be exposed?
For our example:
Safety Impact → Major (vehicle acceleration could be manipulated)
Financial Impact → Moderate (possible warranty or liability issues)
Operational Impact → Moderate (vehicle behavior may become unpredictable)
Privacy Impact → Negligible
From these ratings we derive the overall Impact Level.
➡ Derived Impact Level = Major
📘 Reference Document:
ISO/SAE 21434 – Clause 15 explains how impacts are evaluated and categorized to determine the overall severity of a threat.
🖼 Suggested Visual for Post
(Image idea: Impact rating table with Safety, Financial, Operational, Privacy columns)
________________________________________
4️⃣ Attack Path & Feasibility Analysis 🎯
Next we evaluate how difficult it is for an attacker to perform the attack.
ISO 21434 considers four main factors:
• Elapsed Time – How long it takes to perform the attack
• Expertise – Attacker skill level required
• Knowledge of System – Internal or public information required
• Equipment – Tools needed to perform the attack
Example evaluation:
Elapsed Time → Less than 1 week
Expertise → Proficient attacker
Knowledge → Restricted information required
Equipment → Standard CAN interface tool
From this evaluation we derive the Attack Feasibility Level.
➡ Derived Feasibility Level = 8 (High)
📘 Reference Document:
ISO/SAE 21434 – Clause 15 explains how these factors are combined to determine the difficulty of performing the attack.
🖼 Suggested Visual for Post
(Image idea: Feasibility scoring table or attack path diagram)
________________________________________
5️⃣ Risk Value Calculation 📊
Once the Impact Level and Feasibility Level are known, the risk value can be calculated.
Using the risk matrix method described in ISO/SAE 21434:
Risk is determined by combining Impact Severity and Attack Feasibility.
For our example:
Impact Level → Major
Feasibility Level → 8 (High)
➡ Using the risk determination matrix, the calculated Risk Value = 8
📘 Reference Document:
ISO/SAE 21434 – Clause 15 describes how risk levels are derived using risk matrices or defined project methods.
🖼 Suggested Visual for Post
(Image idea: Risk matrix heatmap showing how Impact and Feasibility produce the Risk value)
________________________________________
6️⃣ Risk Evaluation Against Threshold 🚨
Projects usually define a risk acceptance threshold.
Example threshold:
Risk ≤ 4 → Acceptable
Risk > 4 → Mitigation Required
Since:
Calculated Risk = 8
➡ The risk exceeds the acceptable threshold.
This means cybersecurity mitigation must be implemented.
📘 Reference Document:
ISO/SAE 21434 – Clause 15 explains how calculated risks are compared with acceptance criteria to determine whether mitigation is required.
________________________________________
7️⃣ Engineering Outcome 🔐
From this risk evaluation we derive:
Cybersecurity Goal
Prevent unauthorized modification of the torque request signal.
Cybersecurity Requirement
Implement message authentication and replay protection for the torque request CAN message.
📘 Reference Document:
ISO/SAE 21434 – Clause 9 (Cybersecurity Goals) and Clause 10 (Product Development) describe how security goals and requirements are derived and implemented from the TARA results.
________________________________________
📊 Note
A summary of the complete risk calculation tables (Impact Rating, Attack Feasibility, and Risk Determination) is demonstrated in the Excel sheet used in this example.
________________________________________
💡 Key Insight
Cybersecurity in automotive is not implemented randomly.
It follows a structured engineering process:
Asset → Threat → Impact → Feasibility → Risk → Security Requirement → Implementation
This methodology ensures that security mechanisms are justified by quantified risk, which is the core principle of ISO/SAE 21434.
________________________________________
If you're learning automotive cybersecurity, understanding TARA and risk calculation is one of the most valuable practical skills.
🚗🔐



