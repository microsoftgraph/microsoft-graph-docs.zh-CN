---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc8df128ec1d730296f0ad58480ecc4755f08dc7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328020"
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
result, err := graphClient.IdentityGovernance().TermsOfUse().Agreements().Post(requestBody)


```