---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f17aad2c77beba9585dc4af205c158aa450f293c6e23ab37cb2874707922f8d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.mailAssessmentRequest',
  recipientEmail: 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com',
  expectedAssessment: 'block',
  category: 'spam',
  messageUri: 'https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt='
};

await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```