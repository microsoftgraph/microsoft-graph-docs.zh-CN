---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c11252caacf65e45f537197496cfb0a14da6a6f2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewExtensionProperty()
name := "extensionName"
requestBody.SetName(&name)
dataType := "string"
requestBody.SetDataType(&dataType)
requestBody.SetTargetObjects( []String {
    "Application",
}
options := &msgraphsdk.ExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionProperties().Post(options)


```