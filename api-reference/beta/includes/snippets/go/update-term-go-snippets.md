---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfe6f4327619e7de94ae77a1fd73f3c3438bb3ee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61013704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTerm()
requestBody.SetLabels( []LocalizedLabel {
    msgraphsdk.NewLocalizedLabel(),
    SetAdditionalData(map[string]interface{}{
        "name": "changedLabel",
        "languageTag": "en-US",
        "isDefault": true,
    }
}
options := &msgraphsdk.TermRequestBuilderPatchOptions{
    Body: requestBody,
}
setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Patch(options)


```