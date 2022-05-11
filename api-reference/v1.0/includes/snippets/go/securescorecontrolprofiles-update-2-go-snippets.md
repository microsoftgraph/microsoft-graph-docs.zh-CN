---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1ce5c3226e89eca320410bba9b70f35f2a4ed6b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326958"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecureScoreControlProfile()
vendorInformation := msgraphsdk.NewSecurityVendorInformation()
requestBody.SetVendorInformation(vendorInformation)
provider := "SecureScore"
vendorInformation.SetProvider(&provider)
vendorInformation.SetProviderVersion(nil)
vendorInformation.SetSubProvider(nil)
vendor := "Microsoft"
vendorInformation.SetVendor(&vendor)
requestBody.SetAdditionalData(map[string]interface{}{
    "assignedTo": "",
    "comment": "control is reviewed",
    "state": "Reviewed",
}
secureScoreControlProfileId := "secureScoreControlProfile-id"
graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(requestBody)


```