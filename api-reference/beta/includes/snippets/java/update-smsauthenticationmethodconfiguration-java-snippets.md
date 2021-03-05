---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ddb84918d34ac940db069f41e9bc6a5e37bc05a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475599"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SmsAuthenticationMethodConfiguration authenticationMethodConfiguration = new SmsAuthenticationMethodConfiguration();
authenticationMethodConfiguration.id = "Sms";
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```