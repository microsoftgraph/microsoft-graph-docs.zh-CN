---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50c86240d94228f69a80896ab6459aa97b10fc84
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137760"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName,description,mailNickname",
}
headers := map[string]string{
    "Prefer": "return=minimal"
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Groups().Delta()().Get(options)


```