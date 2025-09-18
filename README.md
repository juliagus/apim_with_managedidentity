# Azure APIM with Managed Identity
How to use Azure APIM and protect APIs with Microsoft Entra ID (using Managed Indentity)

# 1. Configuration of MI and VM
1. Create Managed Identity (no Azure Role Assignments) and record "Client ID" value.
2. VM: create a new VM where you'll run the test code. Note, the testing can only be done from resource in Azure.
3. VM: navigate to "Security" -> "Identity" and assign Managed Identity created at step 1 under "User assigned".

# 2. Policy Configuration at APIM
1. Your API policy should contain the JWT validation policy with required claims.

# 3. Test

# Prerequisite: Basic APIM Configuration
