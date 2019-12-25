---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f00e99958392368b968ee061bd9143bcc817bb9
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new EmailFileAssessmentRequest
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