---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bc3cd4e66fe8b591f91f1733b017502747e4134
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
id := "id-value"
requestBody.SetId(&id)
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
renameAs := "renameAs-value"
requestBody.SetRenameAs(&renameAs)
options := &msgraphsdk.CopyToNotebookRequestBuilderPostOptions{
    Body: requestBody,
}
onenoteSectionId := "onenoteSection-id"
result, err := graphClient.Me().Onenote().SectionsById(&onenoteSectionId).CopyToNotebook(onenoteSection-id).Post(options)


```