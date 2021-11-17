---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed2197f85e6365b2583085f5cbfad9b1c94ce7a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewContactFolder()
displayName := "Family"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ChildFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).ChildFolders().Post(options)


```