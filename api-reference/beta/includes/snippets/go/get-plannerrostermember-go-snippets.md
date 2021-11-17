---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53cdc34b7a66a62f68b9ddd1ff6c9cf6647e7957
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985423"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Get(options)


```