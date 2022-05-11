---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6df1421e48fdbf2a2c77eb3745c08c1b34ad625
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328464"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
content := "Hello world"
body.SetContent(&content)
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Messages().Post(requestBody)


```