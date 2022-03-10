---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf9ac85a6b5582c734cf97ff178f0c1e7c8412ce
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411835"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
keyId := "f0b0b335-1d71-4883-8f98-567911bfdca6"
requestBody.SetKeyId(&keyId)
proof := "eyJ0eXAiOiJ..."
requestBody.SetProof(&proof)
options := &msgraphsdk.RemoveKeyRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).RemoveKey(application-id).Post(options)


```