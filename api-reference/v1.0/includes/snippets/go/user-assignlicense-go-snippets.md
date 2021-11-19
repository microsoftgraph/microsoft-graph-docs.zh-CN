---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71666ec7798d8d9979a1d654d677990aa1808114
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085296"
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
        "skuId": "guid",
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