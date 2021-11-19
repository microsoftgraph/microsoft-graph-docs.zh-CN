---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fbd2520221db4b26405a7ec4c7af975a654e902
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096680"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreement()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isViewingBeforeAcceptanceRequired := true
requestBody.SetIsViewingBeforeAcceptanceRequired(&isViewingBeforeAcceptanceRequired)
options := &msgraphsdk.AgreementRequestBuilderPatchOptions{
    Body: requestBody,
}
agreementId := "agreement-id"
graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Patch(options)


```