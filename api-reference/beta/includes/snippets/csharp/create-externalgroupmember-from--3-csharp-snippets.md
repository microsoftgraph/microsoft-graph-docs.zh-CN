---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0edc5e582678b09cfae6e88a851a77c15374cd7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092126"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new Microsoft.Graph.ExternalConnectors.ExternalGroupMember
{
    Id = "1431b9c38ee647f6a",
    Type = Microsoft.Graph.ExternalConnectors.ExternalGroupMemberType.User
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```