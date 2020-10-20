---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6b6fef0b4ed19651c0f3fad7c659a6e104279aa
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupLifecyclePolicies["{id}"]
    .Request()
    .DeleteAsync();

```