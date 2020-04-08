---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4d96c38aab9b7d9691f2998b7b17050a8a9e38b
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.mailAssessmentRequest",
  recipientEmail: "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  expectedAssessment: "block",
  category: "spam",
  messageUri: "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .version('beta')
    .post(threatAssessmentRequest);

```