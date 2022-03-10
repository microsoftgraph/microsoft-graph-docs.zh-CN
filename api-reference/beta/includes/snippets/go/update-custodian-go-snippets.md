---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c2503309c9e801ea8a94093519d4cea96f31d58
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCustodian()
applyHoldToSources := "false"
requestBody.SetApplyHoldToSources(&applyHoldToSources)
options := &msgraphsdk.CustodianRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).Patch(options)


```