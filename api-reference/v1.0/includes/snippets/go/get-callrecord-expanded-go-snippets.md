---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a884119c2115f27fad260e7e2c0595fc7cc26f6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.CallRecordRequestBuilderGetQueryParameters{
    Expand: "sessions($expand=segments)",
}
options := &msgraphsdk.CallRecordRequestBuilderGetOptions{
    Q: requestParameters,
}
callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).Get(options)


```