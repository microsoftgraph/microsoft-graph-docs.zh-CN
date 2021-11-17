---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b053a304209c39d3d4fb9acb7c275338a97af73962122ee683d20cd8e7544d28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = new PublishedResource
{
    DisplayName = "Demo provisioning (updated)"
};

await graphClient.OnPremisesPublishingProfiles["{onPremisesPublishingProfile-id}"].PublishedResources["{publishedResource-id}"]
    .Request()
    .UpdateAsync(publishedResource);

```