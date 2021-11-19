---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71e1e9cbfad24ab99b47cf1936622d5cef25ccd3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084720"
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
options := &msgraphsdk.SecureScoreControlProfileRequestBuilderPatchOptions{
    Body: requestBody,
}
secureScoreControlProfileId := "secureScoreControlProfile-id"
graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(options)


```