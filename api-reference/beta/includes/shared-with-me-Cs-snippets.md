---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e845e305eb7f10adb4b737b04bd5c6660f0dc84
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457367"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedWithMe = await graphClient.Me.Drive.SharedWithMe()
    .Request()
    .GetAsync();

```