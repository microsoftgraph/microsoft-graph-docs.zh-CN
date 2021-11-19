---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1181e164ffaf0a1a76608e4fafe3c2f0e0d87d8b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093165"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "113feb6c-3fe4-4440-bddc-54d774bf0318",
            "14ab5db5-e6c4-4b20-b4bc-13e36fd2227f",
        }
        "skuId": "b05e124f-c7cc-45a0-a6aa-8cf78c946968",
    }
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "a413a9ff-720c-4822-98ef-2f37c2a21f4c",
        }
        "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    }
}
requestBody.SetRemoveLicenses( []string {
}
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AssignLicense().Post(options)


```