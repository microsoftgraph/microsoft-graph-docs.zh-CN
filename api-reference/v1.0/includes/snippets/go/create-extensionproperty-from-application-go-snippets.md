---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd54145f549178dcbf8b69793de39bd6acde3a92
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326637"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExtensionProperty()
name := "jobGroup"
requestBody.SetName(&name)
dataType := "String"
requestBody.SetDataType(&dataType)
requestBody.SetTargetObjects( []String {
    "User",
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionProperties().Post(requestBody)


```