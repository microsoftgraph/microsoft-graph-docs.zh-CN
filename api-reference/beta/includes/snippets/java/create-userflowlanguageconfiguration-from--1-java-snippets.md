---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bd43bfea7fe605ef54674be38f95c01044af73fd277023752bf63ae0b0a458f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215906"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = new UserFlowLanguageConfiguration();
userFlowLanguageConfiguration.id = "es-ES";
userFlowLanguageConfiguration.isEnabled = true;

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages("es-ES")
    .buildRequest()
    .put(userFlowLanguageConfiguration);

```