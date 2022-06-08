---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6186a091ccf0ec4090b974e0d2007a89f518bfdb
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946839"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRule unifiedRoleManagementPolicyRule = graphClient.policies().roleManagementPolicies("DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448").rules("Expiration_Admin_Eligibility")
    .buildRequest()
    .get();

```