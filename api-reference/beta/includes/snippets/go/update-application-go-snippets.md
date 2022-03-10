---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e51a139f9839849474c6a71253abe0264c7d0705
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411833"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewApplication()
displayName := "New display name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ApplicationRequestBuilderPatchOptions{
    Body: requestBody,
}
applicationId := "application-id"
result, err := graphClient.ApplicationsById(&applicationId).Patch(options)


```