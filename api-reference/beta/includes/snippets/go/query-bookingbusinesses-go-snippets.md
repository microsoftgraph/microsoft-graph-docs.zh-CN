---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39e4cd830f6efac65439bd26b5d71ea710e45fc0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096121"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.BookingBusinessesRequestBuilderGetQueryParameters{
    Query: "Adventure",
}
options := &msgraphsdk.BookingBusinessesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.BookingBusinesses().Get(options)


```