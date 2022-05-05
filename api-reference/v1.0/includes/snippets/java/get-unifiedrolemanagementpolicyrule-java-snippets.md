---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6186a091ccf0ec4090b974e0d2007a89f518bfdb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204463"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRule unifiedRoleManagementPolicyRule = graphClient.policies().roleManagementPolicies("DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448").rules("Expiration_Admin_Eligibility")
    .buildRequest()
    .get();

```