---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0b552cc64f4000231c7ae07f5b796599d18dbc8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSetting cloudPcUserSetting = new CloudPcUserSetting();
cloudPcUserSetting.displayName = "Example";
cloudPcUserSetting.selfServiceEnabled = false;
cloudPcUserSetting.localAdminEnabled = true;

graphClient.deviceManagement().virtualEndpoint().userSettings()
    .buildRequest()
    .post(cloudPcUserSetting);

```