# Dell Storage & Platform Support Account Ranking Prompt
 
Given a list of [[Location & Segment]] companies, rapidly perform:
 
1. Stack rank each company by fit for Dell Storage portfolio, Servers, and platform support:
   - Modern Storage needs (high-performance, scalable, secure)
   - Modern Server needs (high-performance, scalable, secure)
   - Private cloud adoption or interest (VMware, OpenStack, hybrid architectures)
   - Readiness for AIOps/MLOps (automation, AI-driven operations, data pipelines)
   - Dell's integration strengths (PowerFlex, PowerMax, PowerScale, ObjectScale, Compute & Networking, platform tools, multi-cloud support)
 
2. Assign a temperature rating for each company’s likelihood to adopt Dell block storage/private cloud/AIOps/MLOps solutions:
   - 🔥🔥🔥🔥 = Highest (strong Dell fit for storage, cloud, ops automation; clear modernization signals)
   - 🔥🔥🔥 = High (good fit, some cloud adoption or ops innovation; moderate obstacles)
   - 🔥🔥 = Moderate (partial fit for Dell, early cloud/AIOps interest, competitive pressure)
   - 🔥 = Low (limited need or major blockers for Dell solutions)
 
3. Output results in this markdown table:
 
| Rank | Company Name | Industry | Storage/Cloud Readiness | Dell Solution Fit | Temperature | Rationale |
| ---- | ------------ | -------- | ----------------------- | ----------------- | ----------- | --------- |
 
*Optimize for speed. Prioritize Dell’s strengths in Storage, Compute, platform support, private cloud, and AIOps/MLOps alignment when rating accounts.*