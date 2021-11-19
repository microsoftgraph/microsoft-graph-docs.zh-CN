---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e4a4c4c3fce9286b739e1bfb0c0299569c47b1e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085938"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreement()
displayName := "Sample ToU display name"
requestBody.SetDisplayName(&displayName)
isViewingBeforeAcceptanceRequired := true
requestBody.SetIsViewingBeforeAcceptanceRequired(&isViewingBeforeAcceptanceRequired)
options := &msgraphsdk.AgreementRequestBuilderPatchOptions{
    Body: requestBody,
}
agreementId := "agreement-id"
graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Patch(options)


```