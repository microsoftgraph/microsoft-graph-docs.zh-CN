---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ef592a7ee7364b6bd2a065b8e46377d257a4359
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printTaskDefinition = new PrintTaskDefinition
{
    DisplayName = "Test TaskDefinitionName",
    CreatedBy = new AppIdentity
    {
        DisplayName = "Requesting App Display Name"
    }
};

await graphClient.Print.TaskDefinitions
    .Request()
    .AddAsync(printTaskDefinition);

```