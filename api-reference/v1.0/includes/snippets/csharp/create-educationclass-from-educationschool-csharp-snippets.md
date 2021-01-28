---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19692413416f879460673702b657cfe5acd86b74
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"].Users["{user-id}"]
    .Request()
    .DeleteAsync();

```