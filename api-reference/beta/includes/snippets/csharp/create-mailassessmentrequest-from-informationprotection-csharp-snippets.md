---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d6a6580909379c9151ec13ed66b2ffd4722cee
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new MailAssessmentRequest
{
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Spam,
    MessageUri = "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```