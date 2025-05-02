 AI-Powered WAF Bypass using GPT-Neo

## Overview
This project explores bypassing ModSecurity WAF by generating adversarial SQL payloads using GPT-Neo. The environment includes DVWA running on Apache, protected by ModSecurity with custom rules.

## Features
- ModSecurity WAF setup on Apache
- DVWA vulnerable app deployment
- Payload generation using GPT-Neo
- Bypass testing and logging
- Custom WAF rule tuning

## Setup Instructions

1. Install Apache and dependencies
![image](https://github.com/user-attachments/assets/31ebfd42-16f5-4ff8-9c37-ca0c18956bb6)
check Apache whether it is working properly or not
![image](https://github.com/user-attachments/assets/722745be-c4d0-4a87-aab9-962406a9e497)
it will show the default page
![image](https://github.com/user-attachments/assets/1314528c-9f40-40e8-8e8e-5536be69851d)
Install dependencies
![image](https://github.com/user-attachments/assets/b2fd944e-64f5-46b5-89b3-e303bb34846b)

2. Configure ModSecurity and replace with custom rules
  ![image](https://github.com/user-attachments/assets/2fd91253-00ec-43af-8186-faa289e5f856)
 ![image](https://github.com/user-attachments/assets/93b23b11-378c-4c0a-921c-1d836f138747)
![image](https://github.com/user-attachments/assets/328861e2-ae88-416f-9a4a-406b43e6efd8)
![image](https://github.com/user-attachments/assets/a7092024-b587-4618-9081-1096dedfa8f6)
Turn on the secruleengine
![image](https://github.com/user-attachments/assets/44660c12-0976-4062-b07d-2a3bd3d87d8d)
![image](https://github.com/user-attachments/assets/c51880db-be67-42a7-bd39-1bc6c08707ac)
![image](https://github.com/user-attachments/assets/eb8918f3-1dfc-46c5-b5db-375e192f0ce1)

3. Deploy DVWA on local server
![image](https://github.com/user-attachments/assets/829d835d-eb60-436f-a5bb-7303e716f2f2)
![image](https://github.com/user-attachments/assets/e57f2b11-ebbf-45c1-92f5-3914017f8b64)
![image](https://github.com/user-attachments/assets/783f3b1d-7d9a-4dd5-bc69-d75940e57b93)

4. Generate payloads using GPT-Neo
![image](https://github.com/user-attachments/assets/5a603ad7-2906-4cf3-ad62-ecf586d41045)
![image](https://github.com/user-attachments/assets/7074df2b-9617-460c-9f52-12137f91682a)
![image](https://github.com/user-attachments/assets/421fadc0-4246-401a-9d8c-b96b5025299b)

5. Test payloads against the protected web app
Payload - 1
    ![image](https://github.com/user-attachments/assets/8e653907-47f8-4d53-abdb-d68262614633)
result:
![image](https://github.com/user-attachments/assets/8ad51724-1932-4926-bc4b-14d20ef5afbd)
payload-2
![image](https://github.com/user-attachments/assets/1d208981-7708-45d5-a5c4-3e3bf3fe4638)
result:
![image](https://github.com/user-attachments/assets/f5583bc9-9e45-4576-a61a-1716ab9ddb2d)
payload-3
![image](https://github.com/user-attachments/assets/cefbc471-e601-4c8b-8a00-4b7b22004367)
result:
![image](https://github.com/user-attachments/assets/f6b7676c-2e88-4bcd-8c22-718960885ad0)


## Example Payloads

- `selectRow($query, array($id))`
- `SQLite.MySQLSQLDB...`
- `<a href="http://msdn.microsoft.com/...">`

## 📚 Acknowledgements

This project builds upon publicly available resources and tools, including:

- [Damn Vulnerable Web Application (DVWA)](https://github.com/digininja/DVWA)
- [ModSecurity WAF](https://github.com/SpiderLabs/ModSecurity)
- [GPT-Neo by EleutherAI](https://www.eleuther.ai/projects/gpt-neo/)

The configuration, testing, payload generation, and research presented here were performed by me as part of an academic project under the guidance of Mr. Pranjal Upadhyay at Rashtriya Raksha University.

## License
[MIT](LICENSE)

