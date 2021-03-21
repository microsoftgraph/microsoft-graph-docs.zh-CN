---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 006be6e6c48f6670e0c3d24e43f5d4f32893f0eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963209"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HybridAgentUpdaterConfiguration hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration();
UpdateWindow updateWindow = new UpdateWindow();
updateWindow.updateWindowStartTime = new TimeOfDay(0, 0, 0);
updateWindow.updateWindowEndTime = new TimeOfDay(0, 0, 0);
hybridAgentUpdaterConfiguration.updateWindow = updateWindow;

graphClient.customRequest("/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration", HybridAgentUpdaterConfiguration.class)
    .buildRequest()
    .patch(hybridAgentUpdaterConfiguration);

```