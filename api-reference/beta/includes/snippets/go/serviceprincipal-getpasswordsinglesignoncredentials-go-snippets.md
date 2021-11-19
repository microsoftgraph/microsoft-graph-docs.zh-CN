---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a991f7aebdbbd1365233b2f3eadd2fcb69169b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094457"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
options := &msgraphsdk.GetPasswordSingleSignOnCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).GetPasswordSingleSignOnCredentials().Post(options)


```