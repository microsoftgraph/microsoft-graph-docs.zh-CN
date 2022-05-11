---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19d8fad1c12e181788113d7b16153c2e59b2bfd0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315547"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyCollectionPage roleManagementPolicies = graphClient.policies().roleManagementPolicies()
    .buildRequest()
    .filter("scopeId eq '/' and scopeType eq 'Directory'")
    .expand("rules")
    .get();

```