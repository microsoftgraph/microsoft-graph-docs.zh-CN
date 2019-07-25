---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e115d7cfc2269bf2d4dfe2f1aff8360ad19f1de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878250"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HybridAgentUpdaterConfiguration hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration();
hybridAgentUpdaterConfiguration.allowUpdateConfigurationOverride = false;

graphClient.customRequest("/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration", HybridAgentUpdaterConfiguration.class)
    .buildRequest()
    .patch(hybridAgentUpdaterConfiguration);

```