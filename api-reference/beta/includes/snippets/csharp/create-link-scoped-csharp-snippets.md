---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb1b053c3de0a68257ebabac3b2436d84c3e6b92
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,null,null,null)
    .Request()
    .PostAsync();

```