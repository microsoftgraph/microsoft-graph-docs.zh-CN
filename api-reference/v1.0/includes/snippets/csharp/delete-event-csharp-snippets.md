---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e62cd3e02f128f998a75b9e8dac5ecd92780283a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619455"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .Request()
    .DeleteAsync();

```