---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c414a0e59e8e9a207a37f4faf41e7df253d709b0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(null)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```