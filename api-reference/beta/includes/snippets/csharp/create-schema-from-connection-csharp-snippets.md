---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 568736f56fa05ee59f631734299b26b6b2d28d51
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = new Schema
{
    BaseType = "microsoft.graph.externalFile"
};

await graphClient.Connections["contosofiles"].Schema
    .Request()
    .AddAsync(schema);

```