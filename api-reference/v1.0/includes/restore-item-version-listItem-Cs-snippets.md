---
description: 自动生成的文件。 不修改
ms.openlocfilehash: caf21267de7add61c2fc0d560f26bdeab9758c36
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions["{version-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```