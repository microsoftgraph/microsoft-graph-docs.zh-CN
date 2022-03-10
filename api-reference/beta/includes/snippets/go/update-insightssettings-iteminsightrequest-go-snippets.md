---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acec6aaeac574a406f05670aa62e25c8ad2c07d9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411657"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInsightsSettings()
disabledForGroup := "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
requestBody.SetDisabledForGroup(&disabledForGroup)
options := &msgraphsdk.ItemInsightsRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ItemInsights().Patch(options)


```