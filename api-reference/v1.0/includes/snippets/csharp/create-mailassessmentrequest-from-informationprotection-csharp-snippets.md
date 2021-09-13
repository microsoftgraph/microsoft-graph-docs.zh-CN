---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab043067c0c9b18c16b3e4eff2ad84fc475fcfa6bf8927605da06238005a4cdc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new MailAssessmentRequestObject
{
    RecipientEmail = "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Spam,
    MessageUri = "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```