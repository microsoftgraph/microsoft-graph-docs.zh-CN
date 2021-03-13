---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 974e14914a3220048f15cb0082c07e35473dc97a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Versions["{driveItemVersion-id}"]
    .RestoreVersion()
    .Request()
    .PostAsync();

```