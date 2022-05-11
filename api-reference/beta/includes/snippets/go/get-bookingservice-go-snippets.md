---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f90a8217e4689a58e7bda2296250bd0aca30c10
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingServiceId := "bookingService-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).ServicesById(&bookingServiceId).Get()


```