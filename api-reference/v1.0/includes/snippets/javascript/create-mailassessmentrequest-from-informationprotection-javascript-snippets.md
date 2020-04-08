---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1be0ffc755d74185ac9b21fadf72dd7d9a1336f5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815849"
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
  messageUri: "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```