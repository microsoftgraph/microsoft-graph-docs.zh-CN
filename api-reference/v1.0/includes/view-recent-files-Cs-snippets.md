---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 725e70c55100997bf825df7a5a017b74ac83b50e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Drive.Recent()
    .Request()
    .GetAsync();

```