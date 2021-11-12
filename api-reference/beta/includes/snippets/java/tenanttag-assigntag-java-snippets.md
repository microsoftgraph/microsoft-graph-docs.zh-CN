---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba71743d779ef387f28c45b88055eece13359202d5fbe1d5f64955921aab79f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> tenantIdsList = new LinkedList<String>();
tenantIdsList.add("String");

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .assignTag(TenantTagAssignTagParameterSet
        .newBuilder()
        .withTenantIds(tenantIdsList)
        .build())
    .buildRequest()
    .post();

```