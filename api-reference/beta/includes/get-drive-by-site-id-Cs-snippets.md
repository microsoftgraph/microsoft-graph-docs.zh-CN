---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fdcafc495087b78ccc156b4fe25fdcca7b97636d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34483273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{siteId}"].Drive
    .Request()
    .GetAsync();

```