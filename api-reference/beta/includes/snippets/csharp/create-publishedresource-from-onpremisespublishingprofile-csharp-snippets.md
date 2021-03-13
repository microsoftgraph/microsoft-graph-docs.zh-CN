---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8db4cbb7121c09f122e7e8a4035839f534b9dd0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "New provisioning",
    ResourceName = "domain1.contoso.com"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources
    .Request()
    .AddAsync(publishedResource);

```