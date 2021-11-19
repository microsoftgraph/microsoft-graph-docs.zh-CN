---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b6d06d99a7b9a9b3f99af9d691f7c5f9e55b3e5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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