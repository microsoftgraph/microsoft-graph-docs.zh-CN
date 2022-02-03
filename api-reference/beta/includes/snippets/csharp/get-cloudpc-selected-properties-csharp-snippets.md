---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca3bbd1903b5ee4f010215cc1cb3143dab500963
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPC = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Request()
    .Select("id,displayName,imageDisplayName,lastModifiedDateTime,lastRemoteActionResult,lastLoginResult")
    .GetAsync();

```