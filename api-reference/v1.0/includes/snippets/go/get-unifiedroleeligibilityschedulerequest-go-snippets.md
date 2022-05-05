---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94fe6a3b586959e7d3ddd3fe515b4511c50c6cd9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleRequestId := "unifiedRoleEligibilityScheduleRequest-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequestsById(&unifiedRoleEligibilityScheduleRequestId).Get(nil)


```