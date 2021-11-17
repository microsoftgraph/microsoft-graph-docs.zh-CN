---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e376a5007341bc6e32a159f24f530dba7012588
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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