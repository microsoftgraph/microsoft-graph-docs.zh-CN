---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82d8a96c21aae5396d2e8339429f7e57bae8cf09
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613513"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = await graphClient.Me.Drive.Items["{item-id}"].Permissions["{perm-id}"]
    .Request()
    .GetAsync();

```