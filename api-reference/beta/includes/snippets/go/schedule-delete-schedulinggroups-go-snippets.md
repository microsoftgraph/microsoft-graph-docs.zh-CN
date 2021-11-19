---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 614db06f9445b9898e40638c05be5474af124bb0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085006"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Delete(options)


```