---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f4c96356eb5d54e2ef7277340f3a22d23e6c6e1a7c4c15fd498c256cd335ae8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RbacApplicationRoleSchedulesCollectionPage roleSchedules = graphClient.roleManagement().directory()
    .roleSchedules(RbacApplicationRoleSchedulesParameterSet
        .newBuilder()
        .withDirectoryScopeId("a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
        .withAppScopeId("a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
        .withPrincipalId("a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
        .withRoleDefinitionId("a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
        .build())
    .buildRequest()
    .get();

```