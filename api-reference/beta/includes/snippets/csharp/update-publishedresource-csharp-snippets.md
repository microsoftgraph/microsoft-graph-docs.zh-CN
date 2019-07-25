---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f2a5344629f5113a7f0ab367061999cd60c5fa8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874988"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "Demo provisioning (updated)"
};

await graphClient.OnPremisesPublishingProfiles["provisioning"].PublishedResources["1234b780-965f-4149-85c5-a8c73e58b67d"]
    .Request()
    .UpdateAsync(publishedResource);

```