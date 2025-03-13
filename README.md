PERFORMANCE SCIENTIST CASE STUDY

Part 1 – Case Study 

Our Point Guard requests an off-season performance evaluation and program.  She suffered a drop in performance during the previous season. She specifically wants to improve explosiveness coming off screens and getting downhill. She felt slow and had been working with her development coach to improve this. She occasionally battled with Achilles tendon soreness.  She is looking for health, training or lifestyle modifications that could improve performance. 

1.	Using the attached dataset can you describe what you see in the data?
Game Load Data & Data Cleaning Process
•	Game load data was analyzed, and duplicate rows for bodyweight were removed.
•	Missing data was imputed using different methods based on data type:
•	Wellness data: Forward-filling (trends change gradually).
•	Performance metrics: Median imputation (robust to outliers, typically non-normal distribution).
•	Bodyweight: Nearest-neighbor imputation for isolated missing values; z-score outliers were replaced with the mean of surrounding values.
•	Wellness data was not estimated for the All-Star break, assuming no games were played.
•	Bodyweight Imputations: Extreme bodyweight fluctuations were flagged and adjusted based on means of surrounding values:
o	5/13/24 (z-score = -3.05), 6/24/24 (z-score = 1.65), 7/12/24 (z-score = -2.07), and 8/19/24 (z-score = -2.95).
•	Potential Data Error Flagged:
o	5/31/24 bodyweight spike (+11 lbs in 6 days) → Retained but flagged for nutrition staff review (hydration, diet, time of day, shoes on, etc.).
o	5/31 - 6/3 sudden weight drop (-15 lbs) → Unusual (unless travel, illness, menstruation, hydration shifts, etc.), but kept with a flag.
•	CMJ metrics adjusted for bodyweight:
o	RSI, Concentric Impulse, Eccentric Braking Impulse, and Eccentric Peak Velocity recalculated.
o	Peak Power/BM was not adjusted as it inherently accounts for bodyweight.
•	Date Removal:
o	8/4/24 was removed due to: Missing bodyweight data.
o	Key performance outliers:
o	Peak Power/BM (+3.26 z-score), Explosive Efforts (+2.01), Jump Height (-1.99), RSI Modified (+2.45), Eccentric Duration (-2.89), Eccentric Peak Velocity (+1.51).
•	Errors: We chose to use CMJ data but found these conflicting bodyweights below:
6-9-24 – SLJ has bodyweight as 91.03 but CMJ has it at 88.2
7-6-24 – SLJ has bodyweight as 90.94, but CMJ has it at 86.6
8-8-24 – SLJ has bodyweight as 90.90 (no CMJ on that date)
9-1-24 – SLJ has bodyweight at 88.21 (no CMJ on that date)

Can you provide any recommendations for the Health & Performance staff from this data? Please use statistical methods, graphics/visualizations, and code in your explanation 
Achilles Soreness vs Performance Metrics
 
•	Load spikes don’t seem to directly cause soreness the next day or even a few days later or chronic workloads (7-day rolling avg) but soreness did rise in late August, suggesting possible delayed fatigue. 

•	Soreness is influenced by more than just training load with recovery, nutrition, mental fatigue, game scheduling, travel, compensatory movements or asymmetries, etc. as potential contributors.

•	Soreness does not significantly impact explosive performance metrics such as CMJ height, jumps or acceleration. 
Correlation Between Achilles Soreness and Training KPIs  
•	Accels, decel, training loads, distance, and intensity (player load per minute) correlate with lower Achilles soreness (-0.21 to -0.44), suggesting again soreness may be more related to non-training factors rather than overuse or explosive efforts. 








Load Per Distance Before & After Spikes

 
Assuming 6-30-24 load per distance is not a load anomaly, fatigue, or tactical shift (video would allow to see if team played zone or if she played 2 guard, etc. which caused lower load). However, it could be a sign of fatigue or compensation for soreness, but performance and wellness scores do not align.








Load Per Distance vs Decelerations Over Time

 


•	Decels are increasing more than movement efficiency is changing, meaning Load Per Distance is probably not driven by fatigue. 
•	Also suggests improved efficiency or just more decels in less distance, tactical change, defensive adjustment or fatigue compensation.

 
•	Braking force imbalances (Right Achilles) appear to drive power asymmetry the most.
•	Jump Height Asymmetry vs. Peak Power Asymmetry: r = 0.67 (Moderate-Strong Positive)
•	Peak Power Asymmetry vs. Eccentric Braking Asymmetry: r = 0.82 (Strong Positive)
•	RSI asymmetry is more independent, likely influenced by neuromuscular fatigue or other biomechanical factors.











  Asymmetry Testing: Calf Raise Data (9/01
Metric	Left Leg (L)	Right Leg (R)	Asymmetry	Interpretation
Peak Vertical Force (N)	1327	1339	0.9% R	Fairly balanced
Start Time to Peak Force (s)	1.357	2.099	35.3% R	Right Leg taking longer to develop force → Compensation
Rate of Force Development (RFD 200ms)	1238	833	32.7% L	Left Leg producing more explosive force → Right Achilles Weakness
•	R leg has delayed production and produced less explosive force (compensation or weak)
•	L leg is more explosive
________________________________________
Single-Leg CMJ Asymmetry Trends Before & Including 9/1/24
Date	Jump Height Asymm (%)	RSI Asymmetry (%)	Eccentric Braking Asymmetry (%)	Peak Power Asymmetry (%)	Landing Force Asymmetry (%)
6/09	4.4 R	4.3 R	21.5 L	2.6 L	6.9 R
7/06	4.7 R	0.9 L	13 L	2.1 L	9.7 R
8/08	18.2 R	14.6 R	5.7 L	8.6 R	7.6 R
9/01	14 L	22.9 R	32.1 L	4.9 L	4.1	R
•	Left leg is absorbing more braking and jumping force, suggesting compensation for a weaker right leg.
•	Right RSI is increasing, potentially indicating fatigue or increased stiffness.
Braking force and jump asymmetry shifting left suggests a compensatory pattern forming.________________________________________

2.	What other information would supplement your exploration? 

•	Physical and Psychological:
o	Training history overview for this player from Strength & Conditioning 
o	Practice Data: Data appears only to be from games. Practice load is essential for all aspects of a successful athlete monitoring program including readiness, return to play. Tactical, periodization such as tapering before games, and more. (Second Spectrum Optical data available for WNBA?)
o	Past medical history including physical therapy evaluation findings, performance testing, baseline performance profiling, point guard norms, or combine testing, and past performance metrics when not injured.  Medical such as severe dehydration, Illness, or food poisoning.
o	Nutrition and hydration overview from nutritionist: Macronutrient and micronutrient intake 
Longitudinal body composition analysis  
o	Full subjective wellness data that includes psychological factors such as mood/stress for mental resilience and energy/fatigue or RPE but also conversations with the player. 
o	Recovery: modalities utilized along with compliance during the season  

•	Technical and Tactical:
o	Live or recorded game/practice footage with statistics are essential to provide context and observe player movement while analyzing technical and tactical components.
o	Current playing style: Last year, Taurasi and Griner ran a lot of 4 or 5 out and NBA style with fast pace, drive and kicks, iso’s, shooting 3’s - top 5 in attempts per game, protect the rim.
o	Evaluations or conversations with coaches on decision-making, on-court awareness/reaction speed, and efficiency.


________________________________________


3.	How would you present this information to your Health & Performance team-members to optimize this program? Involve each member and collaborate for their discipline 
The full data would be presented to all the members with a collaborative, psychologically safe environment for any questions. 
Physical Therapy/ATC:
Considering HIPAA, we would meet separately to discuss detailed health information unless team standards allow nutritionists, etc. to be a part of the conversation.  A comprehensive summary of the findings would be presented along with possible recommendations. 
Recommend consulting with our physical therapist for a full evaluation to correspond with RLE asymmetry results.
Conversation about possible advanced movement analysis such as Plantiga inserts. 
Our point guard may have good neuromuscular resilience but may be compensating for fatigue through inefficient movement strategies.  

Compensations may not be shown in asymmetry data but could be affecting stride mechanics and ground contact time which can limit explosiveness.

Possible motion capture to assess movement efficiency in-game (NBA biomechanics pilot program in training facilities that includes Suns or something similar?)

Recovery and Resilience: 
Recovery and nutrition appears vital based on the lack of significant findings for much of the existing data. 
How compliant is she with Recovery plan? Create buy-in by finding out what motivates her? 

Sleep and nutrition can take care of up to 90% of recovery and an extra hour of sleep can improve reaction time by up to 20%. 

Options include implementing sleep-tracking (Oura Ring) to optimize recovery or HRV to monitor fatigue.  

Example Plan:
Sleep ✓ You are made to have trouble with quality sleep, so get morning sunlight and try for regular sleep schedule in a cool (62-68 deg), dark, and quiet room. Phone off 1 hr. before bed and use naps from 20-40 min and before 4 pm.
✓ Add Recovery Modalities: Consider what works best for you but these are tiers by proven results Tier 1 - Sleep and nutrition.: Tier 2 - Cryotherapy/Hydrotherapy, Active Recovery (yoga/pool), Massage, Breathwork & Mindfulness, Sauna/BFR/Firefly/Red light. Tier 3 Compression boots, float tanks, cupping, etc.
Nutritionist – Even with only body weight data, nutrition appears to be a focus for our point guard along with the lack of significant data linking workload spikes, soreness, and performance loss. 

How did we address the body weight fluctuations with hydration, meal timing, and recovery nutrition.  
What other tests (hydration testing, InBody testing, questionnaires, meal tracking) to better understand our athlete’s fueling.
Conversation about options including genomic testing to truly understand how the body responds to macronutrients and biomarkers (Vitamin D, Ferritin, Hs-CRP, Testosterone/Cortisol, etc.) to track readiness, recovery, and inflammation. 

Genomics testing: Are you prone to systemic inflammation, low vitamin D, reduced sleep quality/quantity? Does your body respond best to high carbs? 
Performance/S&C -
Conversations and recommendations based on the data along with collaborative approach for clearance from physical therapist/ATC/MD.  
R Achilles tendon health & movement efficiency should be a priority in training design.

The data shows training should focus on improving R eccentric braking mechanics (force absorption) to reduce asymmetry in jump and power production.
With high decel loads late in season: Potential focus should be on braking mechanics, force absorption strategies, and tendon resilience.

Continue monitoring and addressing rate of force development (RFD), RSI, single leg, and bilateral explosiveness to reach player KPI’s

Technical: Needs footwork & acceleration improvements to enhance explosiveness off screens.

Coaching/Tactical: Depending on scheme, analyze screen usage & decision-making under fatigue to optimize downhill attacks.

Final Takeaways

1.	Movement Efficiency & Compensations > Workload Effects
•	The athlete may be compensating for fatigue through inefficient movement strategies rather than showing direct workload effects.
•	Stride length, ground contact time, and foot mechanics could limit explosiveness.
•	No significant impact of workload spikes on soreness, CMJ height, jumps, accelerations, braking force, eccentric strength, or high-load recovery.

2.	Recovery & Non-Physical Stressors
•	Mental fatigue, sleep, travel, & nutrition may be affecting power expression more than workload alone.
•	Load-based soreness effects are inconsistent, highlighting the need for individualized recovery protocols.

3.	R Achilles Tendon Concerns
•	Bodyweight fluctuations (though imputations were required due to errors) may be increasing tendon strain and reducing acceleration.
•	Soreness was not directly linked to workload, but chronic tendon stress could still be a factor.
•	The right Achilles may be at increased risk due to stiffness and force absorption shifts to the left leg, increasing injury risks up the chain.



Part 2 – Short Answer Questions 
1.	What are the key components of an effective athlete monitoring program for professional basketball players?   Because the causes of both injuries and great performance are both multifactorial, an effective athlete monitoring program must be holistic, integrating both physical and psychological components in the embedded department to mitigate injury risk and improve performance.  When utilizing technology, validity, reliability, and independent third-party validation ensures data integrity and actionable insights.  Understanding the game of basketball and the need to just “watch her play” while knowing “context is king” is also a key component. A vital component is the ability to translate the overwhelming volume of data into simple, meaningful outcomes for players and coaches. This ensures that monitoring is actionable, helping players stay healthy, adapt optimally, and perform at their best when it matters most.  The success of any athlete monitoring program depends on buy-in from all stakeholders including players, staff, and coaches and typically includes the following components:
•	Training Load– Monitoring internal and external workload to balance adaptation and injury risk.
•	Neuromuscular Fatigue Monitoring – Force plate testing to track reactive strength, asymmetries, fatigue, and more for readiness.
•	Recovery & Readiness Assessments – Subjective wellness reports, HRV, sleep tracking, and psychological readiness.
•	Nutrition & Hydration Monitoring – Ensuring fueling strategies support recovery and peak performance.
•	Biomechanical & Movement Screening – Assessing joint mobility, asymmetries, ROM, balance, and stability to optimize movement efficiency.
•	Cognitive & Decision-Making Assessments – Evaluating reaction speed, mental fatigue, and decision making with tests such as S2 Cognitive Test.
2.	Can you explain how you use data to drive decision-making in your Health & Performance programs?  I prefer the term data-informed, instead of data-driven.  Sitting behind a computer only tells you part of the story. We must understand the context such as knowing team playing style, on-court observations, and listening to player feedback with conversations.  A data-informed approach ensures that we are not just reacting to numbers but making decisions that align with the realities of the sport, the athlete's needs, and the coaching philosophy.  
For example, a drop in force plate metrics might look concerning in isolation, but without context, we could easily misinterpret it:
•	The athlete may be adjusting to a heavier training block.
•	They might have tested in the morning instead of the afternoon, affecting results.
•	A recent travel stretch could mean they need recovery, not load prescription.

Context is king along with great communication in your collaborative embedded department is vital.  We translate complex data into clear, actionable insights that support coaches and players in training, recovery, and game preparation. Data should enhance decision-making, not replace it.  It’s about building trust with athletes and coaches, so the numbers don’t feel like a judgment, but instead a tool to help them perform at their best. A data-informed approach means blending science, experience, and real human connection. 

3.	Can you provide an example of a successful project or initiative that you led as part of a multi-disciplinary team?   A Power 5 basketball team had no formal sports science program, and I saw an opportunity to help build one from the ground up.  Living in the same town, I started emailing the strength coach and was able to develop a relationship.  He invited me to assist with sports science.  I began meeting with the athletic trainer also.   After attending multiple sports science conferences, I developed relationships with sports science technology companies who had been vetted for reliability and validity.  I reached out to these companies and proposed on-site implementation and real-time integration, which led to a full-season trial with Catapult, despite them rarely offering trials.  After speaking to the strength coach, I convinced him to also add Vald Force Decks.   We had our first “small win” when our former NBA head coach started using real-time practice load data and realized that certain drills were less intense than he originally thought. This built trust in technology, leading to:

•	The coach monitored daily training loads.
•	The athletic trainer used workload data to manage return-to-play protocols.
•	A fully embedded but beginning level sports science workflow.

To improve education and buy in, I launched a weekly sports science email blog for the strength and ATC staff, provided presentations for coaches, interns, and trainers, and gathered feedback to refine our approach.  One very basic example of using data with context involved load asymmetry in practice. We noticed that team load was consistently higher on the left side, leading to several theories—was it injury compensation or an offensive strategy? After watching practice, we realized the managers were running shooting drills only to the left, skewing the data. This reinforced the importance of combining numbers with context.

Another impactful project focused on our best player, who was a high load, “inefficient” mover. I noticed he had unusually high pre-game loads and conducted a small 10-game study to see if this affected his production. Surprisingly, he scored more points on high-load pregame days and had no injuries. This demonstrated that his movement strategy worked for him, preventing unnecessary intervention.
We also used force plate data to monitor asymmetries in an injured player, helping guide his return to play based on his baseline metrics. To streamline onboarding, I created video tutorials and documentation on force plate jump tests, which Vald later used for training materials.

The result? The team renewed its sports science partnership with a paid membership Vald and later transitioned to Kinexon, demonstrating long-term value in the program we implemented.


 



 

