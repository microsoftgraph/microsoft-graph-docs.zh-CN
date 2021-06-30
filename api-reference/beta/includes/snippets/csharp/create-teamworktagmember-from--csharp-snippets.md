---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34dea8e14ca9bc5fdd593e0bf9db3e2514c57af7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamworkTagMember = new TeamworkTagMember
{
    UserId = "97f62344-57dc-409c-88ad-c4af14158ff5"
};

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"].Members
    .Request()
    .AddAsync(teamworkTagMember);

```