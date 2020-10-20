---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e052f9abc42dcdd357eaeef31f818b72cdca9957
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"]
    .Publish()
    .Request()
    .PostAsync();

```