---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f2ab69ffb44c9349e97dee9660497f00477c19f
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountType = CloudPcUserAccountType.Administrator;

var osVersion = CloudPcOperatingSystem.Windows10;

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Reprovision(userAccountType,osVersion)
    .Request()
    .PostAsync();

```