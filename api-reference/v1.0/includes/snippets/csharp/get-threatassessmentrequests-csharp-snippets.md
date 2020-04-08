---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26184a85a8c6e91112261d761d2cbbf338e1e3ea
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815957"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequests = await graphClient.InformationProtection.ThreatAssessmentRequests
    .Request()
    .GetAsync();

```