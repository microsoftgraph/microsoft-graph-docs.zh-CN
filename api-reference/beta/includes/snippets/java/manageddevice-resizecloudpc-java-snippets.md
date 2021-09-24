---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e835d5d1ebd7f29329d83af6abd108250f9a4c34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().managedDevices("{managedDeviceId}")
    .resizeCloudPc(ManagedDeviceResizeCloudPcParameterSet
        .newBuilder()
        .withTargetServicePlanId(null)
        .build())
    .buildRequest()
    .post();

```