---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68eabefd3d5779d7e8d3592b429fc92b47b513af
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsTabId := "teamsTab-id"
result, err := graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Delete(nil)


```