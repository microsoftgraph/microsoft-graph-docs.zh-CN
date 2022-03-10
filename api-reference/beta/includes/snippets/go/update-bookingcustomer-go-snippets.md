---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b04e3cef3d529db74efa8a2ffcd449d1367a18e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412179"
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
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Patch(options)


```