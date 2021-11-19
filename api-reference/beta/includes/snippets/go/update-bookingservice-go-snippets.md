---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaf973208cccb27068a28fd28df1d637eed2e338
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101540"
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
graphClient.BookingBusinessesById(&bookingBusinessId).ServicesById(&bookingServiceId).Patch(options)


```