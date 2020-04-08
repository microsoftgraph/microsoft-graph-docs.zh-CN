---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f2448dc36be67724c06c1a081b64e173e16f01
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  @odata.type: "#microsoft.graph.emailFileAssessmentRequest",
  recipientEmail: "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  expectedAssessment: "block",
  category: "malware",
  contentData: "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
};

let res = await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```