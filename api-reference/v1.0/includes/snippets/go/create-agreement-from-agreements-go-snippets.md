---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9219d8b714e266d4f4c02c7a5c632001aea9a482
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreement()
displayName := "Contoso ToU for guest users"
requestBody.SetDisplayName(&displayName)
isViewingBeforeAcceptanceRequired := true
requestBody.SetIsViewingBeforeAcceptanceRequired(&isViewingBeforeAcceptanceRequired)
requestBody.SetFiles( []AgreementFileLocalization {
    msgraphsdk.NewAgreementFileLocalization(),
    SetAdditionalData(map[string]interface{}{
        "fileName": "TOU.pdf",
        "language": "en",
        "isDefault": true,
    }
}
options := &msgraphsdk.AgreementsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().TermsOfUse().Agreements().Post(options)


```