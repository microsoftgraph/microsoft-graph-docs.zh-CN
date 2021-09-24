---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 605baff80c586f8c93aaebc3183b68307bd046c025b77056cd1040c161674702
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104651"
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