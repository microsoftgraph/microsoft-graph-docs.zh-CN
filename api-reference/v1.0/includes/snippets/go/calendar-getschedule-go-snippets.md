---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b579557e9555d1ddf65c37a6312047f23254feb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetSchedules( []String {
    "adelev@contoso.onmicrosoft.com",
    "meganb@contoso.onmicrosoft.com",
}
startTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStartTime(startTime)
dateTime := "2019-03-15T09:00:00"
startTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
startTime.SetTimeZone(&timeZone)
endTime := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEndTime(endTime)
dateTime := "2019-03-15T18:00:00"
endTime.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
endTime.SetTimeZone(&timeZone)
availabilityViewInterval := int32(60)
requestBody.SetAvailabilityViewInterval(&availabilityViewInterval)
headers := map[string]string{
    "Prefer": "outlook.timezone="Pacific Standard Time""
}
options := &msgraphsdk.GetScheduleRequestBuilderPostOptions{
    Body: requestBody,
    H: headers,
}
result, err := graphClient.Me().Calendar().GetSchedule().Post(options)


```