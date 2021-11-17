---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4656d75feb2190069873dc5d492baeff132f9f0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAgreement()
displayName := "MSGraph Sample"
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