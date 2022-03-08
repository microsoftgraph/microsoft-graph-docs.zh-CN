---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4db0cb2d5b7ed7f021b71310d88fe26196b8003
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().crossTenantAccessPolicy().partners("9c5d131d-b1c3-4fc4-9e3f-c6557947d551")
    .buildRequest()
    .delete();

```