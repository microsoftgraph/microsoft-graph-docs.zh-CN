---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 001cd08f830fdaec7c3cfc99013b2472822c8423
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412335"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DeltaRequestBuilderGetQueryParameters{
    Select: "displayName",
}
headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.DeltaRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).Contacts().Delta()(contactFolder-id).Get(options)


```