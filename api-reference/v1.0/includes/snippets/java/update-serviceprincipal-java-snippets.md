---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17668e484bb25ae1c9f8f316b42878d0787138f8
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334526"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appRoleAssignmentRequired = true;

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .patch(servicePrincipal);

```