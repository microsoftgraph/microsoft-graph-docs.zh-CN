---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ae2d8f5c7c9e7c39636076bf19a87ecd6931d2e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "ocp-client-name": ""My Friendly Client""
    "ocp-client-version": ""1.2""
}
options := &msgraphsdk.RecoveryKeysRequestBuilderGetOptions{
    H: headers,
}
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeys().Get(options)


```