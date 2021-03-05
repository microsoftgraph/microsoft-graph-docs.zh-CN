---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f40da8bbcf05d79af6668241b5925a8dad07571a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = await graphClient.Me.Profile.Anniversaries["{id}"]
    .Request()
    .GetAsync();

```