---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c42dcecf7e7f81b198abecc0f9c3f4eb33b0c6a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327475"
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
connectedOrganizationId := "connectedOrganization-id"
graphClient.IdentityGovernance().EntitlementManagement().ConnectedOrganizationsById(&connectedOrganizationId).Patch(requestBody)


```