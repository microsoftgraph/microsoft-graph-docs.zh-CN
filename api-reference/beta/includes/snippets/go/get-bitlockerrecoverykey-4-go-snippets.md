---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e2053fad737e9582933575d3551874a157a585c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093701"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetQueryParameters{
    Select: "key",
}
options := &msgraphsdk.BitlockerRecoveryKeyRequestBuilderGetOptions{
    Q: requestParameters,
}
bitlockerRecoveryKeyId := "bitlockerRecoveryKey-id"
result, err := graphClient.InformationProtection().Bitlocker().RecoveryKeysById(&bitlockerRecoveryKeyId).Get(options)


```