---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97b36b8f39594e81c36b3c47267080c180715081
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325931"
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
result, err := graphClient.Security().SecurityActions().Post(requestBody)


```