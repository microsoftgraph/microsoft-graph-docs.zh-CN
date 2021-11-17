---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d62153276d15f92bab5d8684f00da4793e8ea4135d45c42dbc241ec95b5cfcb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104174"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleCollectionPage accessPackageResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("beedadfe-01d5-4025-910b-84abb9369997").accessPackageResourceRoles()
    .buildRequest()
    .filter("(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')")
    .select("displayName,originId")
    .get();

```