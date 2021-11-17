---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93fd8cd87a0c935037bfd62f8ea7efd46e7b9064329d9aefab357d6f62da647e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
authorizationPolicy.blockMsolPowerShell = true;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```