---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e819350192b23e9ff7d7df1de2f904f31c38404
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["ab2ad9b3-2213-4091-ae0c-08d76ddbcacf"]
    .Request()
    .GetAsync();

```