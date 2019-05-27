---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ef432fbe22b31ef2661884eaf4da20447d889f2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.DirectoryRoles.Delta()
    .Request()
    .GetAsync();

```