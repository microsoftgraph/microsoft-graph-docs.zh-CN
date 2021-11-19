---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b08cc8d234e16a0f6dbd2cd0153a0a0c0656e8ce
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroup()
description := "Contoso Life v2.0"
requestBody.SetDescription(&description)
displayName := "Contoso Life Renewed"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.GroupRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Patch(options)


```