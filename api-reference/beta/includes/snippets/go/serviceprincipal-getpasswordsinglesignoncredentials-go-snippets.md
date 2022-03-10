---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09752157c519b313b10e87c080c178a8d59931fd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdRequestBody()
id := "5793aa3b-cca9-4794-679a240f8b58"
requestBody.SetId(&id)
options := &msgraphsdk.GetPasswordSingleSignOnCredentialsRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).GetPasswordSingleSignOnCredentials(servicePrincipal-id).Post(options)


```