---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a6fb4c469542d31e1e33ec008bde667defdd6c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608711"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "My custom name";

await graphClient.ApplicationTemplates["{id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```