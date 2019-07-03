---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25f544146d6dcf1f7fc01e497bdb4c0a51945468
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500417"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .GetAsync();

```