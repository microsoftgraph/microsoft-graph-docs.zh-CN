---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07eb1618cd435000efc2a460ec5263eb9cfc90c9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412270"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Publish(bookingBusiness-id).Post(nil)


```