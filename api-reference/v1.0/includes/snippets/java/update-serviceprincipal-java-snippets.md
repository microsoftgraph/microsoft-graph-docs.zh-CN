---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a048a6360ee85afb9f0e6371c32fd3c76fa14561
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appRoleAssignmentRequired = true;

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .patch(servicePrincipal);

```