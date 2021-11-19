---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6092634bc6f24ababd7b2eb920f0634d09b3d5ef
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086629"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
}
options := &msgraphsdk.TeamRequestBuilderPutOptions{
    Body: requestBody,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).Team().Put(options)


```