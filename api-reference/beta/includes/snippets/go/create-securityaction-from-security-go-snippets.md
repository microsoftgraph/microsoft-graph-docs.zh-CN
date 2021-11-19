---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ac19baf856e529e4efaff8415b9026c34fec86c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095931"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSecurityAction()
name := "BlockIp"
requestBody.SetName(&name)
actionReason := "Test"
requestBody.SetActionReason(&actionReason)
requestBody.SetParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "IP",
        "value": "1.2.3.4",
    }
}
vendorInformation := msgraphsdk.NewSecurityVendorInformation()
requestBody.SetVendorInformation(vendorInformation)
provider := "Windows Defender ATP"
vendorInformation.SetProvider(&provider)
vendor := "Microsoft"
vendorInformation.SetVendor(&vendor)
options := &msgraphsdk.SecurityActionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().SecurityActions().Post(options)


```