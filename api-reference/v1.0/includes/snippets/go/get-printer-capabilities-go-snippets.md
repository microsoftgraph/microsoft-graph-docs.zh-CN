---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e74b1f68a0380fd7e3751c46b52173c670ce698a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992635"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PrinterRequestBuilderGetQueryParameters{
    Select: "id,displayName,capabilities",
}
options := &msgraphsdk.PrinterRequestBuilderGetOptions{
    Q: requestParameters,
}
printerId := "printer-id"
result, err := graphClient.Print().PrintersById(&printerId).Get(options)


```