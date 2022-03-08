---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 486795adacf2079f5201ee81d5251825d6cea584
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceIds = new List<String>()
{
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
};

var restorePointDateTime = DateTimeOffset.Parse("2021-09-23T04:00:00");

var timeRange = RestoreTimeRange.Before;

await graphClient.DeviceManagement.ManagedDevices
    .BulkRestoreCloudPc(managedDeviceIds,restorePointDateTime,timeRange)
    .Request()
    .PostAsync();

```