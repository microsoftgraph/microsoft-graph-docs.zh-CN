---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a86378167c5c8878d41c2869f85d60dd6386ca93
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
pkcs12Value := "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA"
requestBody.SetPkcs12Value(&pkcs12Value)
password := "<password>"
requestBody.SetPassword(&password)
options := &msgraphsdk.UploadClientCertificateRequestBuilderPostOptions{
    Body: requestBody,
}
identityApiConnectorId := "identityApiConnector-id"
result, err := graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).UploadClientCertificate(identityApiConnector-id).Post(options)


```