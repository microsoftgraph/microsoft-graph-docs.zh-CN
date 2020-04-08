---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd571d8cb8b630ada5c8d58dfec001f4da6cbbf1
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40871760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = new FileAssessmentRequest
{
    ExpectedAssessment = ThreatExpectedAssessment.Block,
    Category = ThreatCategory.Malware,
    FileName = "test.txt",
    ContentData = "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
};

await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .AddAsync(threatAssessmentRequest);

```