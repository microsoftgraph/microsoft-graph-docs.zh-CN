---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f3fbb4bce03a5368308be34a0e7ec3f72cf0978
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directoryroles["{id}"].Members["{id}"]
    .Request()
    .DeleteAsync();

```