---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 702cd9ecf9e6c1d6279e5308ac5f9e1b003c6a9e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me.FindRooms()
    .Request()
    .GetAsync();

```