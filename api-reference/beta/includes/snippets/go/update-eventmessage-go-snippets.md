---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1303a7fb1adb64aaf81477143cf6cb1f49c693e7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
isRead := "true"
requestBody.SetIsRead(&isRead)
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(requestBody)


```