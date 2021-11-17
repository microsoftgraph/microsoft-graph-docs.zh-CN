---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e106381ec9b5f0f399319875923bdcd795d74043
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990547"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.BookingBusinessesRequestBuilderGetQueryParameters{
    Query: "Adventure",
}
options := &msgraphsdk.BookingBusinessesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.BookingBusinesses().Get(options)


```