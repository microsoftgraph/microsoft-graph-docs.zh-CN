---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 271ece1ba8163bf2e6ac590920ac6cb044e4d13d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524073"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.displayName = "Custom permission grant policy";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy")
    .buildRequest()
    .patch(permissionGrantPolicy);

```