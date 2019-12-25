---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e819350192b23e9ff7d7df1de2f904f31c38404
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867153"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["ab2ad9b3-2213-4091-ae0c-08d76ddbcacf"]
    .Request()
    .GetAsync();

```