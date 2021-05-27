---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e88f3621f8fd1298f45d0e7341131957fd3ac081
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRuleCollectionPage rules = graphClient.policies().roleManagementPolicies("ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba").rules()
    .buildRequest()
    .get();

```