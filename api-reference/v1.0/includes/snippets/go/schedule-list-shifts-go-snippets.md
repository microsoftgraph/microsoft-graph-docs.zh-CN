---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6b2a6e5d4a7cc722d53abc2a71c7c9f428cc8db
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ShiftsRequestBuilderGetQueryParameters{
    Filter: "sharedShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedShift/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftShift/endDateTime%20le%202019-03-18T00:00:00.000Z",
}
options := &msgraphsdk.ShiftsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().Shifts().Get(options)


```