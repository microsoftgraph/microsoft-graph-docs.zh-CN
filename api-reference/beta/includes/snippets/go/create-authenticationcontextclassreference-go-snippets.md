---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eb42a615f7d01e7e5b2f16a74e79ffe93b01e67
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028867"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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