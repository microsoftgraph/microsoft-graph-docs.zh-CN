---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6ac322747a16803151c597c207ab9cd4c14922d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftAuthenticatorAuthenticationMethodConfiguration authenticationMethodConfiguration = new MicrosoftAuthenticatorAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("microsoftAuthenticator")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```