---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d7fd5ae64368f6d7a779c1d82e9c736a793374b3e790465e4a40cb16e2e7a8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378624"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SmsAuthenticationMethodConfiguration authenticationMethodConfiguration = new SmsAuthenticationMethodConfiguration();
authenticationMethodConfiguration.id = "Sms";
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```