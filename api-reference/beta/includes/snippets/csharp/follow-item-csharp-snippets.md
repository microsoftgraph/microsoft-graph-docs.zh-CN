---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3886ccd84da97ff3069d88024ab615822dc5140e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Follow()
    .Request()
    .PostAsync();

```