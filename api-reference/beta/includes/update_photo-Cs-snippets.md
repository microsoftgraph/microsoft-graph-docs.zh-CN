---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d559851524c190907b9454449b511a336a2cd13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profilePhoto = new ProfilePhoto
{
    Height = 99,
    Width = 99,
    Id = "id-value"
};

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .UpdateAsync(profilePhoto);

```