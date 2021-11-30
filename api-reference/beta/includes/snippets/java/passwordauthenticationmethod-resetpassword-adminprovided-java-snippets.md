---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9144523d95aa137c50736a9555874d396e80d33734dd61a8f765d500177c5456
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279114"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String newPassword = "newPassword-value";

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(newPassword)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```