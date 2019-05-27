---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 130de052d6f9e09a2f89001353900cf754bdfa06
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476429"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{special-folder-name}"].Children
    .Request()
    .GetAsync();

```