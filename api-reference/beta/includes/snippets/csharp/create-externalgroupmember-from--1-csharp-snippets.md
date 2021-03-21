---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b9849ee58095babc6e7c99cf1e6e1569e9b4874
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new ExternalGroupMember
{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
    Type = ExternalGroupMemberType.User,
    IdentitySource = IdentitySourceType.AzureActiveDirectory
};

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```