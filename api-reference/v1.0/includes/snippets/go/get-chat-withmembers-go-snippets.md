---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8faa1d528debd8cb30d61c128e7162d007d9e25
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326240"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```