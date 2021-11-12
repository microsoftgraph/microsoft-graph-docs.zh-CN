---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0da2f177d149c9a4ab43b0579caa039149a999a3bf036e43f91078f2c2dc1cc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> tenantIdsList = new LinkedList<String>();
tenantIdsList.add("String");

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .unassignTag(TenantTagUnassignTagParameterSet
        .newBuilder()
        .withTenantIds(tenantIdsList)
        .build())
    .buildRequest()
    .post();

```