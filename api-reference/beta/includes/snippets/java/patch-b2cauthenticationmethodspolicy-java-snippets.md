---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f10f60eb9eb0d719d33e2e557f474d3b68fc5138
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081502"
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