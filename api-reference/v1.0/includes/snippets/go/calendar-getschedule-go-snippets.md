---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adcf6c86e457ca1f49f660896eb2296e2c03a65d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082318"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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