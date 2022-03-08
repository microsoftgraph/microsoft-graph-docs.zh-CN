---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0527903ac580aba26a168001dea9b8423a955a7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336569"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicy crossTenantAccessPolicy = graphClient.policies().crossTenantAccessPolicy()
    .buildRequest()
    .get();

```