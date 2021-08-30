---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 415bfe05029e1c02db07ead1db74d26e813853ca791e36511ef7485fb49ed3d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105280"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cAuthenticationMethodsPolicy b2cAuthenticationMethodsPolicy = new B2cAuthenticationMethodsPolicy();
b2cAuthenticationMethodsPolicy.isEmailPasswordAuthenticationEnabled = false;
b2cAuthenticationMethodsPolicy.isUserNameAuthenticationEnabled = true;
b2cAuthenticationMethodsPolicy.isPhoneOneTimePasswordAuthenticationEnabled = true;

graphClient.policies().b2cAuthenticationMethodsPolicy()
    .buildRequest()
    .patch(b2cAuthenticationMethodsPolicy);

```