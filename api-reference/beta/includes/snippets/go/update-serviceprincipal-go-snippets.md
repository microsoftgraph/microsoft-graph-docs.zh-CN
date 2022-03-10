---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a642db7b19fd2f932c854c2522c184583b6791f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewServicePrincipal()
appRoleAssignmentRequired := true
requestBody.SetAppRoleAssignmentRequired(&appRoleAssignmentRequired)
options := &msgraphsdk.ServicePrincipalRequestBuilderPatchOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Patch(options)


```