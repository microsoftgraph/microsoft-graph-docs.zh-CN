---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f68e89795211ddb5a6f3e4427802a413c23a403b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474683"
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