---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbbe2380317dd88ee7607a7044ee872039743f39
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactFolder()
displayName := "Family"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ChildFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
contactFolderId := "contactFolder-id"
result, err := graphClient.Me().ContactFoldersById(&contactFolderId).ChildFolders().Post(options)


```