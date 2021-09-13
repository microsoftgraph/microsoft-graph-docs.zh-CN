---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e628928fdb0a7dd0ab91da939dcb8631a4315ccc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identity = new Microsoft.Graph.ExternalConnectors.Identity
{
    Id = "e811976d-83df-4cbd-8b9b-5215b18aa874",
    Type = Microsoft.Graph.ExternalConnectors.IdentityType.User
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"].Members
    .Request()
    .AddAsync(identity);

```