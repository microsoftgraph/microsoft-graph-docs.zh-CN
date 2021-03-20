---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e57461a6a03d87491fdc03ae2dac341e941970a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944633"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = new UserFlowLanguageConfiguration();
userFlowLanguageConfiguration.isEnabled = false;

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages("es-ES")
    .buildRequest()
    .put(userFlowLanguageConfiguration);

```