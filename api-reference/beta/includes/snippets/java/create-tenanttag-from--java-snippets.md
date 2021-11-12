---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee5899b0404f90ae585a6d290756478996a221e4e29b5ad28ed36aa05cc497d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158522"
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