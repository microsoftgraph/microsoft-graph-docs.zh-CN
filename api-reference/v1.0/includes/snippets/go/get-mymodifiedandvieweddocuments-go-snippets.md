---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef801f2e9b75e605384e0b5843a273838bc3326
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085330"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsedRequestBuilderGetQueryParameters{
    Orderby: "LastUsed/LastAccessedDateTime%20desc",
}
options := &msgraphsdk.UsedRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().Insights().Used().Get(options)


```