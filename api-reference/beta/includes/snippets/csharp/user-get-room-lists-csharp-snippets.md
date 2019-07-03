---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b26c76d2aa31188f948665765326b3de612540dc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521302"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRoomLists = await graphClient.Me.FindRoomLists()
    .Request()
    .GetAsync();

```