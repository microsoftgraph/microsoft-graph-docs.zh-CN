---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dffaee27fa5c0ce2719101dd8f7dab32e7663b7b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411656"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInsightsSettings()
isEnabledInOrganization := true
requestBody.SetIsEnabledInOrganization(&isEnabledInOrganization)
disabledForGroup := "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
requestBody.SetDisabledForGroup(&disabledForGroup)
options := &msgraphsdk.PeopleInsightsRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().PeopleInsights().Patch(options)


```