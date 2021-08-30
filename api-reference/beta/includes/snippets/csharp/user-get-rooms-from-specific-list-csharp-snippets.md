---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c02790ea2804b227fcb64457271c8de8523ffa54cb92eb3b1c817578a598efd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var findRooms = await graphClient.Me
    .FindRooms("Building2Rooms@contoso.onmicrosoft.com")
    .Request()
    .GetAsync();

```