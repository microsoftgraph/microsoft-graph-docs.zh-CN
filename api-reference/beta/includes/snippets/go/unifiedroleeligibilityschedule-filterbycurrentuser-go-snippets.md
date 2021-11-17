---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac9807a8ee1d10cbfbb6e99e7127f5601d6f61c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016973"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleEligibilityScheduleId := "unifiedRoleEligibilitySchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilitySchedulesById(&unifiedRoleEligibilityScheduleId).Get(options)


```