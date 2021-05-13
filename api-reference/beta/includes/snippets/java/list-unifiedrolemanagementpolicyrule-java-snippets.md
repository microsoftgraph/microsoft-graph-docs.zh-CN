---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d187d52691224e3573e29afe65eabed0bab55374
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474282"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRuleCollectionPage effectiveRules = graphClient.policies().roleManagementPolicies("ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba").effectiveRules()
    .buildRequest()
    .get();

```