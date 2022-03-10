---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6feefbbb10db38ea0b5292d9cec15b37b4624a4
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411771"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactFolder()
parentFolderId := "parentFolderId-value"
requestBody.SetParentFolderId(&parentFolderId)
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ContactFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).Patch(options)


```