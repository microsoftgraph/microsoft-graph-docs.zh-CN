---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 273921dab668b5b947287cbbd82e7889da1ddc5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}.Content
    .Request()
    .GetAsync();

```