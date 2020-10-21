---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f544146d6dcf1f7fc01e497bdb4c0a51945468
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .GetAsync();

```