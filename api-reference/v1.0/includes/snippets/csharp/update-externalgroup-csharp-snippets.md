---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0584086857b4dbdadc18825af3ba5cb0d8fdda3a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalGroup = new Microsoft.Graph.ExternalConnectors.ExternalGroup
{
    DisplayName = "Contoso Marketing",
    Description = "The product marketing team"
};

await graphClient.Connections["{externalConnectors.externalConnection-id}"].Groups["{externalConnectors.externalGroup-id}"]
    .Request()
    .UpdateAsync(externalGroup);

```