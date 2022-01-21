---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e6dffbce7ac27289a7a2fa80c66c9f5f13affe9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,null,null,null,null,null,null)
    .Request()
    .PostAsync();

```