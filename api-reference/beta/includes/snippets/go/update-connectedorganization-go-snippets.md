---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66267faa9e326cb68dbf13b3843de7c00793abd2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097602"
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
graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Patch(options)


```