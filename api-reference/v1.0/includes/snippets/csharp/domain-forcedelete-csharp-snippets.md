---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e5c597c2af5f5a78120a3b5bb2b51acbf97b411
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var disableUserAccounts = true;

await graphClient.Domains["{id}"]
    .ForceDelete(disableUserAccounts)
    .Request()
    .PostAsync();

```