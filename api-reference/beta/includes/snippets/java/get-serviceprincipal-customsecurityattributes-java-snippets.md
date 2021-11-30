---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a5970bb8a0e6097e5bfb2d2524928a83151ac88
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226264"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = graphClient.servicePrincipals("{id}")
    .buildRequest()
    .select("customSecurityAttributes")
    .get();

```