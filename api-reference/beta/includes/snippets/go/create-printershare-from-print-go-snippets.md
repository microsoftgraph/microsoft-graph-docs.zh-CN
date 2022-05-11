---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1618c2a3205a9f48a94ac9d5d271542ee0ae4d5a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrinterShare()
name := "name-value"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}",
}
result, err := graphClient.Print().Shares().Post(requestBody)


```