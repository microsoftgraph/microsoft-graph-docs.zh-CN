---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f24b6840a51883c1133c8936a928b6d45a069c3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AgreementRequestBuilderGetQueryParameters{
    Expand: "files",
}
options := &msgraphsdk.AgreementRequestBuilderGetOptions{
    Q: requestParameters,
}
agreementId := "agreement-id"
result, err := graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Get(options)


```