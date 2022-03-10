---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f06202fd9115394c12b45078cca44d33a85b788
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412513"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
options := &msgraphsdk.ForwardRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).Forward(group-id, conversationThread-id, post-id).Post(options)


```