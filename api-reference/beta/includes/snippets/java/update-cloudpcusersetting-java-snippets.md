---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a4b7f8310bda8726995c536f2922cab8aab7f2b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335491"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSetting cloudPcUserSetting = new CloudPcUserSetting();
cloudPcUserSetting.displayName = "Example";
cloudPcUserSetting.selfServiceEnabled = true;
CloudPcRestorePointSetting restorePointSetting = new CloudPcRestorePointSetting();
restorePointSetting.frequencyInHours = "16";
restorePointSetting.userRestoreEnabled = true;
cloudPcUserSetting.restorePointSetting = restorePointSetting;
cloudPcUserSetting.localAdminEnabled = false;

graphClient.deviceManagement().virtualEndpoint().userSettings("b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff")
    .buildRequest()
    .patch(cloudPcUserSetting);

```