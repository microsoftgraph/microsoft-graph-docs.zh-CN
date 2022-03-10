---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0833b48dc54ca73d657c11d27f3f088a37c47580
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412080"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewKeyIdRequestBody()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
options := &msgraphsdk.RemovePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).RemovePassword(application-id).Post(options)


```