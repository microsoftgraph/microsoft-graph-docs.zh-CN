---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aef63df593c5eae0af2012b7a4c57538ad82e7d5
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867150"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["49c5ef5b-1f65-444a-e6b9-08d772ea2059"]
    .Request()
    .GetAsync();

```