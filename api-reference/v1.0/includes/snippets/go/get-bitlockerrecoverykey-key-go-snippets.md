---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2907a4fb2c9b5444d380765c4dfb44e189a31207
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001105"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetQueryParameters{
    Select: "key",
}
options := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetOptions{
    Q: requestParameters,
}
bitlockerRecoveryKeyId := "bitlockerRecoveryKey-id"
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeysById(&bitlockerRecoveryKeyId).Get(options)


```