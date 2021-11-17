---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96616e503367060b86e2fd222b944dc158d9600b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981489"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.RefRequestBuilderDeleteQueryParameters{
    Id: "https://graph.microsoft.com/beta/users/%7Bid%7D",
}
options := &msgraphsdk.RefRequestBuilderDeleteOptions{
    Q: requestParameters,
}
groupId := "group-id"
graphClient.GroupsById(&groupId).RejectedSenders().$ref().Delete(options)


```