---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9af7a1e558ad4b02c386af93dcfdde470da39af8491480f94084c5fd4c7b366
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new Microsoft.Graph.ExternalConnectors.ExternalGroupMember
{
    Id = "1431b9c38ee647f6a",
    Type = Microsoft.Graph.ExternalConnectors.ExternalGroupMemberType.Group,
    IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.External
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```