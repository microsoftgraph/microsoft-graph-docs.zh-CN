---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d0de9a626b7a64986f7571c3c7cad298da34112
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979087"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
authorizationPolicy.blockMsolPowerShell = true;

graphClient.policies().authorizationPolicy()
    .buildRequest()
    .patch(authorizationPolicy);

```