---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb4d59e3659691032bea600ea138fb9c0893a5ee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010119"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
        }
        "skuId": "skuId-value-1",
    }
    msgraphsdk.NewAssignedLicense(),
    SetAdditionalData(map[string]interface{}{
        "disabledPlans":  []String {
            "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235",
        }
        "skuId": "skuId-value-2",
    }
}
requestBody.SetRemoveLicenses( []string {
}
options := &msgraphsdk.AssignLicenseRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().AssignLicense().Post(options)


```