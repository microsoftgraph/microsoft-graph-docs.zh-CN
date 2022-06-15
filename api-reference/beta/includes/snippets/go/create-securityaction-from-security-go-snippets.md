---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc532dc3d5293c495c7d6e8d85d0ee773f057123
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098695"
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
name := "IP"
    SetName(&name)
value := "1.2.3.4"
    SetValue(&value)
}
vendorInformation := msgraphsdk.NewSecurityVendorInformation()
requestBody.SetVendorInformation(vendorInformation)
provider := "Windows Defender ATP"
vendorInformation.SetProvider(&provider)
vendor := "Microsoft"
vendorInformation.SetVendor(&vendor)
result, err := graphClient.Security().SecurityActions().Post(requestBody)


```