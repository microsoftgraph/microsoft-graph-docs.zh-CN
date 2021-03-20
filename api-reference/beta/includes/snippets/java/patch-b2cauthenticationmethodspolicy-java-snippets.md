---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78330e09624351880ea3f382a41b4e6175712f04
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970565"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cAuthenticationMethodsPolicy b2cAuthenticationMethodsPolicy = new B2cAuthenticationMethodsPolicy();
b2cAuthenticationMethodsPolicy.isEmailPasswordAuthenticationEnabled = false;
b2cAuthenticationMethodsPolicy.isUserNameAuthenticationEnabled = true;

graphClient.policies().b2cAuthenticationMethodsPolicy()
    .buildRequest()
    .patch(b2cAuthenticationMethodsPolicy);

```