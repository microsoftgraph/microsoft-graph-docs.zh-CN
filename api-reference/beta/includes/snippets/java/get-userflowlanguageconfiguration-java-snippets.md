---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e83bb6d24c1f3eb4787e8a0da3028de54823b7c7
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274936"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp").languages()
    .buildRequest()
    .get();

```