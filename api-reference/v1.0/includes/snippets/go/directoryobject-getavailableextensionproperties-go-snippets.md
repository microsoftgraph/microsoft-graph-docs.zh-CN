---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43ba31b074a1aeeddf943e2d38c5b4f49bbb0b22
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412125"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIsSyncedFromOnPremisesRequestBody()
isSyncedFromOnPremises := true
requestBody.SetIsSyncedFromOnPremises(&isSyncedFromOnPremises)
options := &msgraphsdk.GetAvailableExtensionPropertiesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.DirectoryObjects().GetAvailableExtensionProperties().Post(options)


```