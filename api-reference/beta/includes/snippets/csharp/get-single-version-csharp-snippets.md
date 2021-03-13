---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded05bdb5a8cb9560e28aba423006fc62ce5bdf3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790296"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItemVersion = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions["{driveItemVersion-id}"]
    .Request()
    .GetAsync();

```