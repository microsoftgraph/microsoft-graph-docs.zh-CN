---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f53e1010a16233271f3b114f080344c2b5eb7d0f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412717"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Delete(nil)


```