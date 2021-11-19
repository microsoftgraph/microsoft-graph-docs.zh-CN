---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 557f7df90acd29ca74d36112ba36ed4bcd3b167d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083700"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PrinterRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterRequestBuilderGetOptions{
    Q: requestParameters,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Get(options)


```