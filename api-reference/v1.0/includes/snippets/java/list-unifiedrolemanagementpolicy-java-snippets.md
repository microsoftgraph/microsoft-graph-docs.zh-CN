---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9ae2832ea9b8a5532576df672a6c6d9a963c618
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyCollectionPage roleManagementPolicies = graphClient.policies().roleManagementPolicies()
    .buildRequest()
    .filter("scopeId eq '/' and scopeType eq 'DirectoryRole'")
    .get();

```