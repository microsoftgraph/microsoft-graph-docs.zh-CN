---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e429d8f324c334d5a7f5c2bd609ccae3f76b1a4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkout()
    .Request()
    .PostAsync();

```