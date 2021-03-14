---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91c6a48bc8607ee218ba527bcf5ed25c5b590306
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const threatAssessmentRequest = {
  '@odata.type': '#microsoft.graph.emailFileAssessmentRequest',
  recipientEmail: 'tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com',
  expectedAssessment: 'block',
  category: 'malware',
  contentData: 'UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC.....'
};

await client.api('/informationProtection/threatAssessmentRequests')
    .post(threatAssessmentRequest);

```