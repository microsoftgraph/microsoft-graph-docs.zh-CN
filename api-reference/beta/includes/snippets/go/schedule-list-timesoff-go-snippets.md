---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 774166417e5435c3a92380868ef6578f31e156cf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093405"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TimesOffRequestBuilderGetQueryParameters{
    Filter: "sharedTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z",
}
options := &msgraphsdk.TimesOffRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimesOff().Get(options)


```