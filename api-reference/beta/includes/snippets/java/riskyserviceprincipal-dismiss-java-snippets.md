---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f12f63a54c0fa7711815520ad6846a7957716dc9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> servicePrincipalIdsList = new LinkedList<String>();
servicePrincipalIdsList.add("9089a539-a539-9089-39a5-899039a58990");

graphClient.identityProtection().riskyServicePrincipals()
    .dismiss(RiskyServicePrincipalDismissParameterSet
        .newBuilder()
        .withServicePrincipalIds(servicePrincipalIdsList)
        .build())
    .buildRequest()
    .post();

```