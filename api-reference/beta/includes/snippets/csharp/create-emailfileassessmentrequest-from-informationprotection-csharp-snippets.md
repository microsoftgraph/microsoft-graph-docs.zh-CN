---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d63cd0a797a0aa93e0a51d1bc124098049738977
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new EmailFileAssessmentRequestObject
{
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Malware,
    ContentData = "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```