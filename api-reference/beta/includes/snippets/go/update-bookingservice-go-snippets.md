---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ae0676d600434ed6fbe283ffb8eb8aff5d5ad4f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411779"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingService()
defaultDuration := "PT30M"
requestBody.SetDefaultDuration(&defaultDuration)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingService",
}
options := &msgraphsdk.BookingServiceRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingServiceId := "bookingService-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).ServicesById(&bookingServiceId).Patch(options)


```