---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d80bdf5c4c1c92fa2e974cae96aa5fd65771ccf30a36daa0e011d8cd6fc45a49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328919"
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