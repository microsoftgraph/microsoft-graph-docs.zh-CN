---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab8568457effa23e38628228614735d0938363e5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990644"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.CalendarViewRequestBuilderGetQueryParameters{
    Start: "2018-04-30T00:00:00Z",
    End: "2018-05-10T00:00:00Z",
}
options := &msgraphsdk.CalendarViewRequestBuilderGetOptions{
    Q: requestParameters,
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CalendarView().Get(options)


```