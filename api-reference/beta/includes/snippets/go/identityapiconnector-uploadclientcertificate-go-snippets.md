---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7af02f1e0be9f586d89389cddc6b94d42987de9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095566"
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
result, err := graphClient.Identity().ApiConnectorsById(&identityApiConnectorId).UploadClientCertificate().Post(options)


```