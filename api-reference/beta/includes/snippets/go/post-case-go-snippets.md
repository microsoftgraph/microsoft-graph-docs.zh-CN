---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 386adee4cfbcc66118c36ba514143861ee27525f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100227"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCase()
displayName := "My Case 1"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.CasesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Compliance().Ediscovery().Cases().Post(options)


```