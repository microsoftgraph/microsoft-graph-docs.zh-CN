---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7951f12578b9ccad09ec2143f45c33f0e1b3e4eac58aba2bed43823d61f56cd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161437"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = new B2cIdentityUserFlow();
b2cIdentityUserFlow.id = "Customer";
b2cIdentityUserFlow.userFlowType = UserFlowType.SIGN_UP_OR_SIGN_IN;
b2cIdentityUserFlow.userFlowTypeVersion = 3;

graphClient.identity().b2cUserFlows()
    .buildRequest()
    .post(b2cIdentityUserFlow);

```