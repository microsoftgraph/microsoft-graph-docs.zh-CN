---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50bd7256f129949f579c83497838602f1bbe51d1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438650"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserSource()
email := "admin@M365x809305.onmicrosoft.com"
requestBody.SetEmail(&email)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryHoldPolicyId := "ediscoveryHoldPolicy-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).LegalHoldsById(&ediscoveryHoldPolicyId).UserSources().Post(requestBody)


```