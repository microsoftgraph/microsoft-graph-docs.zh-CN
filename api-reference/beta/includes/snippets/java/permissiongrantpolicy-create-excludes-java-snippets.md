---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46f560ea3b547607cd36b52e8c884d127bf8e757
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969295"
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