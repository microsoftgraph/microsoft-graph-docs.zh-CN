---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d072d78c1d50b52d550e60527f5f5c3a54d9d2f4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336457"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicyConfigurationDefault crossTenantAccessPolicyConfigurationDefault = graphClient.policies().crossTenantAccessPolicy().default()
    .buildRequest()
    .get();

```