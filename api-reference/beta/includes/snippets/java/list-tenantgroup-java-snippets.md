---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77bce3ff6d1af849199e88639e2941951a7b5ecca32da3695e13f37dbed6bc11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106644"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantGroupCollectionPage tenantGroups = graphClient.tenantRelationships().managedTenants().tenantGroups()
    .buildRequest()
    .get();

```