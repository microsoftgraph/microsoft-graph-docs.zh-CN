---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc1e2c62e60db88b8c700e1bffa2025474e9f6d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59508690"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().managedDevices("{managedDeviceId}")
    .reprovisionCloudPc()
    .buildRequest()
    .post();

```