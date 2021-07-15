---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2434a88ce6b9e2fbb829085fd84268001ff33312
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439262"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRoleCollectionPage accessPackageResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("beedadfe-01d5-4025-910b-84abb9369997").accessPackageResourceRoles()
    .buildRequest()
    .filter("(originSystem eq 'SharePointOnline' and accessPackageResource/id eq '53c71803-a0a8-4777-aecc-075de8ee3991')")
    .select("displayName,originId")
    .get();

```