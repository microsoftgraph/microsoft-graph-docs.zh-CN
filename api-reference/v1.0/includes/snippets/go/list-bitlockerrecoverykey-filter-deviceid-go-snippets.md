---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e297ec9e3f70ca8a45be3a6f7639adc84424a5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001148"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RecoveryKeysRequestBuilderGetQueryParameters{
    Filter: "deviceId%20eq%20'1ab40ab2-32a8-4b00-b6b5-ba724e407de9'",
}
headers := map[string]string{
    "ocp-client-name": ""My Friendly Client""
    "ocp-client-version": ""1.2""
}
options := &msgraphsdk.RecoveryKeysRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeys().Get(options)


```