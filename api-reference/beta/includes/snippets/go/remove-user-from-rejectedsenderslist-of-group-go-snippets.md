---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23d93122d8af7341901c504a10e9713f42a4ea8a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412588"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/beta/users/%7Bid%7D",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).RejectedSendersById(&directoryObjectId).Delete(options)


```