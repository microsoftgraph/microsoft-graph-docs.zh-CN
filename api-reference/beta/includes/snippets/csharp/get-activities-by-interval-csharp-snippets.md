---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ea9f1a9477695c0906922641b1464356d7e22cd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785766"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getActivitiesByInterval = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .GetActivitiesByInterval("2017-01-01","2017-01-3","day")
    .Request()
    .GetAsync();

```