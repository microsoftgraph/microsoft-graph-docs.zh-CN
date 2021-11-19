---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1d0150a1751898ee3f854583151ba5a859eaae4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094489"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Get(options)


```