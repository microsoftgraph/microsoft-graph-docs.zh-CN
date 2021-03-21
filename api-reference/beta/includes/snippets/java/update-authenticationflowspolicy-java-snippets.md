---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4243e55845b5e654228589e993a2ed410ac09b08
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationFlowsPolicy authenticationFlowsPolicy = new AuthenticationFlowsPolicy();
SelfServiceSignUpAuthenticationFlowConfiguration selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
selfServiceSignUp.isEnabled = true;
authenticationFlowsPolicy.selfServiceSignUp = selfServiceSignUp;

graphClient.policies().authenticationFlowsPolicy()
    .buildRequest()
    .patch(authenticationFlowsPolicy);

```