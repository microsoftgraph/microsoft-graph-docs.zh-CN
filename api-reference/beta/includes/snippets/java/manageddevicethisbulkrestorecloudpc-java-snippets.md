---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eca3f71116b4097b08ee72feb1c75dac5b5087dc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338188"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> managedDeviceIdsList = new LinkedList<String>();
managedDeviceIdsList.add("30d0e128-de93-41dc-89ec-33d84bb662a0");
managedDeviceIdsList.add("7c82a3e3-9459-44e4-94d9-b92f93bf78dd");

OffsetDateTime restorePointDateTime = OffsetDateTimeSerializer.deserialize("09/23/2021 04:00:00");

RestoreTimeRange timeRange = RestoreTimeRange.BEFORE;

graphClient.deviceManagement().managedDevices()
    .bulkRestoreCloudPc(ManagedDeviceBulkRestoreCloudPcParameterSet
        .newBuilder()
        .withManagedDeviceIds(managedDeviceIdsList)
        .withRestorePointDateTime(restorePointDateTime)
        .withTimeRange(timeRange)
        .build())
    .buildRequest()
    .post();

```