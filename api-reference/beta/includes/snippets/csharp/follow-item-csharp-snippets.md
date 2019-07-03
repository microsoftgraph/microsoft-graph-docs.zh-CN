---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f82cb90fcecd47d6f218a9d12b1dfa6a1908264
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Follow()
    .Request()
    .PostAsync();

```