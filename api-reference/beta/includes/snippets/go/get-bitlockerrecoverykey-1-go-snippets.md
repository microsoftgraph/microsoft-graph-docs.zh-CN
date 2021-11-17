---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d39e21944c73f0f0f8b39bffbed542b7a1ae1da2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60999755"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

headers := map[string]string{
    "ocp-client-name": ""My Friendly Client""
    "ocp-client-version": ""1.2""
}
options := &msgraphsdk.RecoveryKeysRequestBuilderGetOptions{
    H: headers,
}
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeys().Get(options)


```