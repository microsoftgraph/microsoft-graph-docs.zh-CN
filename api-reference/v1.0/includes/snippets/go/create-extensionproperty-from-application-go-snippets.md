---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90f55a5d2e54f9e3ca8ac90ce9334cd79a583da7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412475"
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
options := &msgraphsdk.ExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionProperties().Post(options)


```