---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47649ec1ec26b97e65453fc7acc3028a63e65407
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327204"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomer()
displayName := "Adele"
requestBody.SetDisplayName(&displayName)
emailAddress := "adele@relecloud.com"
requestBody.SetEmailAddress(&emailAddress)
bookingBusinessId := "bookingBusiness-id"
bookingCustomerId := "bookingCustomer-id"
graphClient.BookingBusinessesById(&bookingBusinessId).CustomersById(&bookingCustomerId).Patch(requestBody)


```