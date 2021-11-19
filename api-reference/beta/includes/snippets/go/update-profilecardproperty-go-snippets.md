---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51ee83f3dff9359eb4648c211639c352db0f18de
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090558"
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
graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Patch(options)


```