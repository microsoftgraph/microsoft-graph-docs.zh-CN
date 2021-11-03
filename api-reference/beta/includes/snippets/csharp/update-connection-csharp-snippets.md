---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2adbcb9fade777828c285906466ca99728b24ab7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689105"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalConnection = new Microsoft.Graph.ExternalConnectors.ExternalConnection
{
    Name = "Contoso HR Service Tickets",
    Description = "Connection to index HR service tickets"
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"]
    .Request()
    .UpdateAsync(externalConnection);

```