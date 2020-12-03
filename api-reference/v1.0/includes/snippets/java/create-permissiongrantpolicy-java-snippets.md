---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddab776ccb2eb8aa5344ad505efa698398fb164d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524116"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantPolicy permissionGrantPolicy = new PermissionGrantPolicy();
permissionGrantPolicy.id = "my-custom-consent-policy";
permissionGrantPolicy.displayName = "Custom application consent policy";
permissionGrantPolicy.description = "A custom permission grant policy to customize conditions for granting consent.";

graphClient.policies().permissionGrantPolicies()
    .buildRequest()
    .post(permissionGrantPolicy);

```