---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf8ba27f0a7d11043da086295e25139bd8140709
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().appManagementPolicies("{id}")
    .buildRequest()
    .delete();

```