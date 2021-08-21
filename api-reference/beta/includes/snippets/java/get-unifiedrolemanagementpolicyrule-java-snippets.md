---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6be52f355ed62e8020a41e1bd88e90a83f88941a01f147b5181b5c4c362138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRule unifiedRoleManagementPolicyRule = graphClient.policies().roleManagementPolicies("{unifiedRoleManagementPolicyId}").rules("{unifiedRoleManagementPolicyRuleId}")
    .buildRequest()
    .get();

```