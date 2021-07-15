---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a6d78719c411f237f81b5de102fcc17815fb301
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440906"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantGroupId = "String";

String tenantId = "String";

String managementActionId = "String";

String managementTemplateId = "String";

String status = "String";

graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses()
    .changeDeploymentStatus(ManagementActionTenantDeploymentStatusChangeDeploymentStatusParameterSet
        .newBuilder()
        .withTenantGroupId(tenantGroupId)
        .withTenantId(tenantId)
        .withManagementActionId(managementActionId)
        .withManagementTemplateId(managementTemplateId)
        .withStatus(status)
        .build())
    .buildRequest()
    .post();

```