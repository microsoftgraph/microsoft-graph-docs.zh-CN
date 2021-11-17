---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e5841598f4667b1844778820655fcc034249783
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034071"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Expand: "extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```