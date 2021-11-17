---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 217badda317b8bec25584323bc269a9ecec635d0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026345"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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