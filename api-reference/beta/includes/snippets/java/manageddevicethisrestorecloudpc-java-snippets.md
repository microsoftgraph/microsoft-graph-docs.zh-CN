---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 087e84c2ad6171746fa3e09e72da78033ee4a2e7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338877"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String cloudPcSnapshotId = "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8";

graphClient.deviceManagement().managedDevices("5e1387aa-d960-4916-ae7c-293b977e49bf")
    .restoreCloudPc(ManagedDeviceRestoreCloudPcParameterSet
        .newBuilder()
        .withCloudPcSnapshotId(cloudPcSnapshotId)
        .build())
    .buildRequest()
    .post();

```