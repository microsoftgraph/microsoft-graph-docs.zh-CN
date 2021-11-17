---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9da9250e6eca9b34419e7b5e3e6811bf78ea7390
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantId = "String";

String tenantGroupId = "String";

String managementTemplateId = "String";

graphClient.tenantRelationships().managedTenants().managementActions("{managementActionId}")
    .apply(ManagementActionApplyParameterSet
        .newBuilder()
        .withTenantId(tenantId)
        .withTenantGroupId(tenantGroupId)
        .withManagementTemplateId(managementTemplateId)
        .withIncludeAllUsers(null)
        .withIncludeGroups(null)
        .withExcludeGroups(null)
        .build())
    .buildRequest()
    .post();

```