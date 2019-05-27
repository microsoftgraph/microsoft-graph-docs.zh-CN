---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef1d0938090343a4388b9249921fe0a72d538f40
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{object-id}"]
    .Request()
    .DeleteAsync();

```