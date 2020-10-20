---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f21fe4aa3646cdac9f1b2e1f3a7a9b0fc10478a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = await graphClient.SchemaExtensions["graphlearn_test"]
    .Request()
    .GetAsync();

```