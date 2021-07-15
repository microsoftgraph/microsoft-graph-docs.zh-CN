---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9972510124e88404f037216ff53bee4cd806362
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTag tenantTag = new TenantTag();
tenantTag.displayName = "Support";
tenantTag.description = "Tenants that have purchased extended support";

graphClient.tenantRelationships().managedTenants().tenantTags()
    .buildRequest()
    .post(tenantTag);

```