---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6528615c7ed222fad6c37a09697128a006f32b40
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274906"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlow identityUserFlow = new IdentityUserFlow();
identityUserFlow.id = "Pol1";
identityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
identityUserFlow.userFlowTypeVersion = 1;

graphClient.identity().userFlows()
    .buildRequest()
    .post(identityUserFlow);

```