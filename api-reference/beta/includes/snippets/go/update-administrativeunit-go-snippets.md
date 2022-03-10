---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27d0562f10cb21dd4e6a7e8929a1b8f7fb048382
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411850"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "Greater Seattle District Technical Schools"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AdministrativeUnitRequestBuilderPatchOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.AdministrativeUnitsById(&administrativeUnitId).Patch(options)


```