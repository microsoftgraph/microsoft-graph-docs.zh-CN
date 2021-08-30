---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72fe8400a9b5d3c5e142f82f483d08a1082a25680480b53ef4e479cf2cd6f8d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new Microsoft.Graph.ExternalConnectors.ExternalGroupMember
{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
    Type = Microsoft.Graph.ExternalConnectors.ExternalGroupMemberType.User,
    IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.AzureActiveDirectory
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```