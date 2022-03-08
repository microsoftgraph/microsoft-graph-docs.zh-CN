---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 067af659f7dbe20804bf43412f331eed09582541
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337346"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyServicePrincipalCollectionPage riskyServicePrincipals = graphClient.identityProtection().riskyServicePrincipals()
    .buildRequest()
    .get();

```