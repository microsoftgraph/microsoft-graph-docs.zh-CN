---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd929e8707252cd8620075f87aeaed27d051ed1a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonCertification()
issuingAuthority := "International Academy of Marketing Excellence"
requestBody.SetIssuingAuthority(&issuingAuthority)
issuingCompany := "International Academy of Marketing Excellence"
requestBody.SetIssuingCompany(&issuingCompany)
options := &msgraphsdk.PersonCertificationRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
personCertificationId := "personCertification-id"
result, err := graphClient.UsersById(&userId).Profile().CertificationsById(&personCertificationId).Patch(options)


```