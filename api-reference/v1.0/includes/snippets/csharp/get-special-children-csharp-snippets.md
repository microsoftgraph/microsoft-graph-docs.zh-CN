---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a8d44da2bdd7445e0477e8641259c4ac4751abc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Special["{driveItem-id}"].Children
    .Request()
    .GetAsync();

```