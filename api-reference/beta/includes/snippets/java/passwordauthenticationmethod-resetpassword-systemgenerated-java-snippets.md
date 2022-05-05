---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf16bd21e1d4e79c61cc7823b524349b866882de
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220313"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0").authentication().passwordMethods("28c10230-6103-485e-b985-444c60001490")
    .resetPassword(AuthenticationMethodResetPasswordParameterSet
        .newBuilder()
        .withNewPassword(null)
        .withRequireChangeOnNextSignIn(null)
        .build())
    .buildRequest()
    .post();

```