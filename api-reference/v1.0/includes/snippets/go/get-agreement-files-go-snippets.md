---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f24b6840a51883c1133c8936a928b6d45a069c3
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515816"
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