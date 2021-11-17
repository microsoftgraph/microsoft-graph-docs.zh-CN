---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6edfe4cf4b27eb4b80291b150f3fec43df79c4a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60978702"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PrinterShareRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterShareRequestBuilderGetOptions{
    Q: requestParameters,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).Get(options)


```