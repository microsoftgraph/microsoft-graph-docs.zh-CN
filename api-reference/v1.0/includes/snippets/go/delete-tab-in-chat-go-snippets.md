---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfe4d8d52f321bd004e82f9794a57d61cc9f3a4d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974340"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
teamsTabId := "teamsTab-id"
graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Delete(options)


```