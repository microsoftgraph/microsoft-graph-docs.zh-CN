---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a58c44b523fb4540c76622b87087ee7295f2ee46
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewVerifiedPublisherIdRequestBody()
verifiedPublisherId := "1234567"
requestBody.SetVerifiedPublisherId(&verifiedPublisherId)
options := &msgraphsdk.SetVerifiedPublisherRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).SetVerifiedPublisher(application-id).Post(options)


```