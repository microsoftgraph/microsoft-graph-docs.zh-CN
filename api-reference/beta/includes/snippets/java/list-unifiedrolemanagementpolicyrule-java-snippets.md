---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9472b6f8bed9e4b740dc31f3efc5b92a321eb5c5
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319516"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyRuleCollectionPage rules = graphClient.policies().roleManagementPolicies("{unifiedRoleManagementPolicyId}").rules()
    .buildRequest()
    .get();

```