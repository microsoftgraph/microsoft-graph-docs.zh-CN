---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3db9d304903fa4b2c87babac7348c7fa47848f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220281"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOrganizationSettings cloudPcOrganizationSettings = new CloudPcOrganizationSettings();
cloudPcOrganizationSettings.userAccountType = CloudPcUserAccountType.STANDARD_USER;
cloudPcOrganizationSettings.osVersion = CloudPcOperatingSystem.WINDOWS11;
CloudPcWindowsSettings windowsSettings = new CloudPcWindowsSettings();
windowsSettings.language = "en-US";
cloudPcOrganizationSettings.windowsSettings = windowsSettings;

graphClient.deviceManagement().virtualEndpoint().organizationSettings()
    .buildRequest()
    .patch(cloudPcOrganizationSettings);

```