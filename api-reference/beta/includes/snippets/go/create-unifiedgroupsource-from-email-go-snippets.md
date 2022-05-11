---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9d86abaac6a8c440d4003eb8196338780f33abc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328415"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedGroupSource()
group := msgraphsdk.NewGroup()
requestBody.SetGroup(group)
mail := "SecretGroup@contoso.com"
group.SetMail(&mail)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSources().Post(requestBody)


```