---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46f560ea3b547607cd36b52e8c884d127bf8e757
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524191"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSet permissionGrantConditionSet = new PermissionGrantConditionSet();
permissionGrantConditionSet.permissionType = PermissionType.DELEGATED;
permissionGrantConditionSet.resourceApplication = "00000003-0000-0000-c000-000000000000";

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").excludes()
    .buildRequest()
    .post(permissionGrantConditionSet);

```