---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c92213968ae6fa3ba9bc56a367173571ff63edc
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334665"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyServicePrincipal riskyServicePrincipal = graphClient.identityProtection().riskyServicePrincipals("9089a539-a539-9089-39a5-899039a58990")
    .buildRequest()
    .get();

```