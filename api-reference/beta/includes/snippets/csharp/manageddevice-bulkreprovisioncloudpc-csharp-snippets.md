---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fb600f47eba7c56ea13505fad1e7c2efaec09f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59507895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceIds = new List<String>()
{
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
};

await graphClient.DeviceManagement.ManagedDevices
    .BulkReprovisionCloudPc(managedDeviceIds)
    .Request()
    .PostAsync();

```