---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d9dfd5fb4f32aa2facb184200a158782c140077
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524136"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSet permissionGrantConditionSet = new PermissionGrantConditionSet();
permissionGrantConditionSet.permissionType = PermissionType.DELEGATED;
permissionGrantConditionSet.clientApplicationsFromVerifiedPublisherOnly = true;

graphClient.policies().permissionGrantPolicies("{id}").includes()
    .buildRequest()
    .post(permissionGrantConditionSet);

```