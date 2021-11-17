---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 324872a80cf22a88ec7ced29c1617eaf53c9b1a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ShiftsRequestBuilderGetQueryParameters{
    Filter: "sharedShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedShift/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftShift/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftShift/endDateTime%20le%202019-03-18T00:00:00.000Z",
}
options := &msgraphsdk.ShiftsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().Shifts().Get(options)


```