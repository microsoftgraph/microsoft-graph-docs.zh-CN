---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5983dece366268bb29eb23d5c44a43c4608a7150
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210218"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HybridAgentUpdaterConfiguration hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration();
UpdateWindow updateWindow = new UpdateWindow();
updateWindow.updateWindowStartTime = new TimeOfDay(0, 0, 0);
updateWindow.updateWindowEndTime = new TimeOfDay(0, 0, 0);
hybridAgentUpdaterConfiguration.updateWindow = updateWindow;

graphClient.customRequest("/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration", HybridAgentUpdaterConfiguration.class)
    .buildRequest()
    .patch(hybridAgentUpdaterConfiguration);

```