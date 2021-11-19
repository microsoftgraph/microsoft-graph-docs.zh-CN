---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f58b3e36905a4e80ddcf48cb3fd154bb243e64
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserSource()
email := "megan@contoso.com"
requestBody.SetEmail(&email)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
options := &msgraphsdk.UserSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UserSources().Post(options)


```