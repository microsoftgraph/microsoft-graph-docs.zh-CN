---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 969939e411797d7bedbe5a534ce6cb247b78a3f1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089301"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RefRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/v1.0/users/%7Buser-id%7D",
}
options := &msgraphsdk.RefRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).RejectedSenders().$ref().Delete(options)


```