---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c290a2e42da8afaaa01869f90423f67da68021ab
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412133"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConnectedOrganization()
displayName := "Connected organization new name"
requestBody.SetDisplayName(&displayName)
description := "Connected organization new description"
requestBody.SetDescription(&description)
state := "configured"
requestBody.SetState(&state)
options := &msgraphsdk.ConnectedOrganizationRequestBuilderPatchOptions{
    Body: requestBody,
}
connectedOrganizationId := "connectedOrganization-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Patch(options)


```