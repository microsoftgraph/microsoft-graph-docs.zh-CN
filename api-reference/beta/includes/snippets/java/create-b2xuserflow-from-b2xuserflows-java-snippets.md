---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33e0c8b11254a7aa99a3f892f1c576149cbebeb0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2xIdentityUserFlow b2xIdentityUserFlow = new B2xIdentityUserFlow();
b2xIdentityUserFlow.id = "Partner";
b2xIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2xIdentityUserFlow.userFlowTypeVersion = 1;

graphClient.identity().b2xUserFlows()
    .buildRequest()
    .post(b2xIdentityUserFlow);

```