---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cf9b2a122f19e5f8903cb960328f93b09fefe3d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987466"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
description := "description-value"
requestBody.SetDescription(&description)
visibility := "visibility-value"
requestBody.SetVisibility(&visibility)
options := &msgraphsdk.AdministrativeUnitRequestBuilderPatchOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Patch(options)


```