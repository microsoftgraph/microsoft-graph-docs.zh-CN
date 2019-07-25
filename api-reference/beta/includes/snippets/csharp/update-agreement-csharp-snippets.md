---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 667322331d4082546634e12b8187ceb2e1efbb4e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "displayName-value",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.Agreements["'id'"]
    .Request()
    .UpdateAsync(agreement);

```