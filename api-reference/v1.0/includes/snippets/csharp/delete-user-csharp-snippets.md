---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 02727a1c2499e558f1d2b6584ccf7a2c4f55a9b7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```