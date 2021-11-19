---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48eb1d18d702b36d31f1b96bcc05e6e66885c05e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090109"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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