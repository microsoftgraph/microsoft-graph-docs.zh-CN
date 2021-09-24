---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 531103d71cddb8348cbd74df4ad30086202829cf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59507905"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> managedDeviceIdsList = new LinkedList<String>();
managedDeviceIdsList.add("30d0e128-de93-41dc-89ec-33d84bb662a0");
managedDeviceIdsList.add("7c82a3e3-9459-44e4-94d9-b92f93bf78dd");

graphClient.deviceManagement().managedDevices()
    .bulkReprovisionCloudPc(ManagedDeviceBulkReprovisionCloudPcParameterSet
        .newBuilder()
        .withManagedDeviceIds(managedDeviceIdsList)
        .build())
    .buildRequest()
    .post();

```