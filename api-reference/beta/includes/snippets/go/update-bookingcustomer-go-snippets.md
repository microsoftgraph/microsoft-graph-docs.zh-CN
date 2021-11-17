---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40678fcab40cefff3d6c1318840900aa0ed5f884
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990483"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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