---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 158e0f06760193edd921893f09e55c8654cb347f
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "1431b9c38ee647f6a",
    Type = ExternalGroupMemberType.Group,
    IdentitySource = IdentitySourceType.External
};

await graphClient.External.Connections["contosohr"].Groups["31bea3d537902000"].Members
    .Request()
    .AddAsync(externalGroupMember);

```