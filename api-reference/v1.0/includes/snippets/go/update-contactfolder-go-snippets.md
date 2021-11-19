---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54b62d2a030bfe92913dd72f7dc26555e936be83
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103085"
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
graphClient.Me().ContactFoldersById(&contactFolderId).Patch(options)


```