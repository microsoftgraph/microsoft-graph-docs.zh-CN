---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b384b5b6742c765cae96ccf53f3d303dcc6c3ffc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Special["{name}"]
    .Request()
    .GetAsync();

```