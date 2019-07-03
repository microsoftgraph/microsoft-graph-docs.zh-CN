---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a2135be2fa313fd8cee336096932609a25f7c53
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {size} = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}
    .Request()
    .GetAsync();

```