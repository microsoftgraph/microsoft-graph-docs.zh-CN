---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e925140c473fd0059e771b2394edd5ace91e95a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new UrlAssessmentRequest
{
    Url = "http://test.com",
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Phishing
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```