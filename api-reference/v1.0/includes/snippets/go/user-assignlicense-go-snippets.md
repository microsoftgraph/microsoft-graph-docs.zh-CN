---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86e2cbb5c0219c05dc51d3d302b7741d3bcd4758
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336800"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
        }
        "skuId": "45715bb8-13f9-4bf6-927f-ef96c102d394",
    }
}
requestBody.SetRemoveLicenses( []String {
    "bea13e0c-3828-4daa-a392-28af7ff61a0f",
}
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().AssignLicense().Post(options)


```