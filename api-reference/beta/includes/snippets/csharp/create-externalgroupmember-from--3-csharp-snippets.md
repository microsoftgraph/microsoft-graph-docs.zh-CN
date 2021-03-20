---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e111ef2ddae3fdee9954dd845c83ca068a5ccd09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956006"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "1431b9c38ee647f6a",
    Type = ExternalGroupMemberType.Group,
    IdentitySource = IdentitySourceType.External
};

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```