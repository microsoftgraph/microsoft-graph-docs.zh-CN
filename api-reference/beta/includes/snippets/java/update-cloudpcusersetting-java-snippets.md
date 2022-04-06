---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71c0f7b0d5e10dd3b412fe26cde02b0345f166e4
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSetting cloudPcUserSetting = new CloudPcUserSetting();
cloudPcUserSetting.displayName = "Example";
cloudPcUserSetting.selfServiceEnabled = true;
CloudPcRestorePointSetting restorePointSetting = new CloudPcRestorePointSetting();
restorePointSetting.frequencyInHours = 16;
restorePointSetting.userRestoreEnabled = true;
cloudPcUserSetting.restorePointSetting = restorePointSetting;
cloudPcUserSetting.localAdminEnabled = false;

graphClient.deviceManagement().virtualEndpoint().userSettings("b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff")
    .buildRequest()
    .patch(cloudPcUserSetting);

```