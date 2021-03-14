---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ca82436b1206cab85e4af60ef0352c18b651e84
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Versions["{driveItemVersion-id}"].Content
    .Request()
    .GetAsync();

```