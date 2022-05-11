---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b73fcb401765f0eb5ab1d9dff6d2beb668e10a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamworkTagMember()
userId := "97f62344-57dc-409c-88ad-c4af14158ff5"
requestBody.SetUserId(&userId)
teamId := "team-id"
teamworkTagId := "teamworkTag-id"
result, err := graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Members().Post(requestBody)


```