---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cb61f8b4cca2245e9a749f5c6fdc1cc980f1114
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087039"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthenticationContextClassReference()
id := "c1"
requestBody.SetId(&id)
displayName := "Contoso medium"
requestBody.SetDisplayName(&displayName)
description := "Medium protection level defined for Contoso policy"
requestBody.SetDescription(&description)
isAvailable := true
requestBody.SetIsAvailable(&isAvailable)
options := &msgraphsdk.AuthenticationContextClassReferencesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferences().Post(options)


```