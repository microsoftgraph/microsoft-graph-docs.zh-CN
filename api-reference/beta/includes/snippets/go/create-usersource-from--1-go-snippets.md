---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2bcdcf9683d4b5fb73dbcffe1d9d659d9189a6b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserSource()
email := "megan@contoso.com"
requestBody.SetEmail(&email)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UserSources().Post(requestBody)


```