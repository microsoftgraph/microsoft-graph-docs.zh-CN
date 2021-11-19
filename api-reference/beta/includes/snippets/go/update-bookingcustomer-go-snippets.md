---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 712e7aebacbd3c763b6e79a620faed14db615caa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomer()
displayName := "Adele"
requestBody.SetDisplayName(&displayName)
emailAddress := "adele@relecloud.com"
requestBody.SetEmailAddress(&emailAddress)
options := &msgraphsdk.BookingCustomerRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingCustomerId := "bookingCustomer-id"
graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Patch(options)


```