---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b29942e80d70a9d95189a8b9ecb0076bf75cfbc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.TiIndicatorRequestBuilderPatchOptions{
    H: headers,
}
tiIndicatorId := "tiIndicator-id"
graphClient.Security().TiIndicatorsById(&tiIndicatorId).Patch(options)


```