---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e859fb62e53fc3dd524b41bb932bb6578bc81800
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096425"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleRequestId := "unifiedRoleEligibilityScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleEligibilityScheduleRequestsById(&unifiedRoleEligibilityScheduleRequestId).Cancel().Post(options)


```