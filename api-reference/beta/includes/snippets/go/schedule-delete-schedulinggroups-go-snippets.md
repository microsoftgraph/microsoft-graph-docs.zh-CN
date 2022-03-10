---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 873927cec8d72d14177b2efa46e0070e709bc178
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Delete(nil)


```