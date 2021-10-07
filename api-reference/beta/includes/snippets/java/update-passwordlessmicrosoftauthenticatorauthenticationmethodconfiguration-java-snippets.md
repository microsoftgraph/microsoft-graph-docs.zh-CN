---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 969dbca2acb3a4dea82b1becd90898ee8206402ea70634329d9b74943d128128
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104375"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration authenticationMethodConfiguration = new PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("passwordlessMicrosoftAuthenticator")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```