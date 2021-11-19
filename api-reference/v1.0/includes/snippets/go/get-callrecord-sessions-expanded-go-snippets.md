---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3956a23c4aa05099d0c2815529999f427f037601
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098178"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SessionsRequestBuilderGetQueryParameters{
    Expand: "segments",
}
options := &msgraphsdk.SessionsRequestBuilderGetOptions{
    Q: requestParameters,
}
callRecordId := "callRecord-id"
result, err := graphClient.Communications().CallRecordsById(&callRecordId).Sessions().Get(options)


```