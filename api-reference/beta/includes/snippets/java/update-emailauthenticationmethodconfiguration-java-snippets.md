---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61c48c693bef96252a26aa037f02d30f08ff72e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776338"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethodConfiguration authenticationMethodConfiguration = new EmailAuthenticationMethodConfiguration();
authenticationMethodConfiguration.allowExternalIdToUseEmailOtp = ExternalEmailOtpState.DEFAULT;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```