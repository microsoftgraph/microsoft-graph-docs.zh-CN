---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e39e9dbbc54d5703ba1c540c2e8508d327eb16f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookingCurrencyId := "bookingCurrency-id"
result, err := graphClient.BookingCurrenciesById(&bookingCurrencyId).Get(options)


```