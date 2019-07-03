---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d559851524c190907b9454449b511a336a2cd13
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493042"
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