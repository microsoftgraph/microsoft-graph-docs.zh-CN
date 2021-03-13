---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad5a665e5cee940ce44527ddac836be35b3fa440
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{driveItem-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```