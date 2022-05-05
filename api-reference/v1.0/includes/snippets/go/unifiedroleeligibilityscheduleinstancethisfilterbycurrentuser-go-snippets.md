---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76f730cc119ac30f96303be7e3dfc0fe80d713ee
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204930"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleInstanceId := "unifiedRoleEligibilityScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleInstancesById(&unifiedRoleEligibilityScheduleInstanceId).Get(nil)


```