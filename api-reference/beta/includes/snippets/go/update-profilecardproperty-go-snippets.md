---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20af6a4caa22ad1372868762cc8c29b23af015f9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412352"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProfileCardProperty()
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
    SetAdditionalData(map[string]interface{}{
        "localizations":  []Object {
        }
    }
}
options := &msgraphsdk.ProfileCardPropertyRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Patch(options)


```