---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10a3ba20e17476f146ef07eb83405df89f0a404b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412208"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DirectoryObjectRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).AcceptedSendersById(&directoryObjectId).Delete(options)


```