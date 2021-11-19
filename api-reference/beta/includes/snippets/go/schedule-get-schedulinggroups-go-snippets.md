---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4370e1bf942e7319282212f0f862b0497291f84c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101130"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Get(options)


```