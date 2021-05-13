---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a395e33438bec94df364798701cd5271402c51
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474767"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRule unifiedRoleManagementPolicyRule = graphClient.policies().roleManagementPolicies("{unifiedRoleManagementPolicyId}").rules("{unifiedRoleManagementPolicyRuleId}")
    .buildRequest()
    .get();

```