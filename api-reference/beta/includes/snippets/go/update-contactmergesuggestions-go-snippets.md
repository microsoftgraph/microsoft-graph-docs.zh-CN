---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5324e130ef195c11fdb969b9e2828d9bfc1f3e6f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528165"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactMergeSuggestions()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.ContactMergeSuggestionsRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Settings().ContactMergeSuggestions().Patch(options)


```