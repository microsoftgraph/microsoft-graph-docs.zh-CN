---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2b95762613622fdba524205757fe1ee7de6daf33c1571badf82e3e244d79a71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroupMember = new Microsoft.Graph.ExternalConnectors.ExternalGroupMember
{
    Id = "e5477431-1038-484e-bf69-1dfedb97a110",
    Type = Microsoft.Graph.ExternalConnectors.ExternalGroupMemberType.Group,
    IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.AzureActiveDirectory
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(externalGroupMember);

```