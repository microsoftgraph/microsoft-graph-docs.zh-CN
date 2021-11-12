---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c1905bb967762215541bf0198e3e44d532cb72430c2e8de1aa94c196317cc69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158372"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantId = "String";

graphClient.tenantRelationships().managedTenants().tenantGroups()
    .tenantSearch(TenantGroupTenantSearchParameterSet
        .newBuilder()
        .withTenantId(tenantId)
        .build())
    .buildRequest()
    .post();

```