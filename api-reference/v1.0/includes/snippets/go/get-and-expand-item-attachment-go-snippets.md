---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58cbdab96475ea292e9c32fa6b0957a58927d04c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327093"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AttachmentRequestBuilderGetQueryParameters{
    Expand: "microsoft.graph.itemattachment/item",
}
options := &msgraphsdk.AttachmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
messageId := "message-id"
attachmentId := "attachment-id"
result, err := graphClient.Me().MessagesById(&messageId).AttachmentsById(&attachmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```