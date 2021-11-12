---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ae5a237d702e191ff2a6e59936d67a8444ee4f7c28c0396953123fde5c94bea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163969"
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
        .build())
    .buildRequest()
    .post();

```