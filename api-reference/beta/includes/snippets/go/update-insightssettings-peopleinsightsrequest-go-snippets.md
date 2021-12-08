---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9811c9018318912d91f04ee755ee02402684ec41
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61339517"
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
graphClient.OrganizationById(&organizationId).Settings().PeopleInsights().Patch(options)


```