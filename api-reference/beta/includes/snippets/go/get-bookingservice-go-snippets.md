---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8cc0fed827727d87e4b7aee7820709e0621927a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096109"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
bookingServiceId := "bookingService-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).ServicesById(&bookingServiceId).Get(options)


```