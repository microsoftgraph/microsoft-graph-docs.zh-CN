---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e06a69ba6a385f933eb36a81241802fc106a41f3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077305"
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
graphClient.ServicePrincipalsById(&servicePrincipalId).Patch(options)


```