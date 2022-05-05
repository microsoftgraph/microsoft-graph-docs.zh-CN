---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdd71a9116d876cc529d9059b65f10f7c2c7b83f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().entitlementManagement().roleAssignments()
    .buildRequest()
    .filter("appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'")
    .expand("principal")
    .get();

```