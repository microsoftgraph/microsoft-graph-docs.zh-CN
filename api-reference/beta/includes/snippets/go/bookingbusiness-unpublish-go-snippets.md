---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 863d4257f73642b57ab8c12fcb72364f3c175997
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Unpublish(bookingBusiness-id).Post(nil)


```