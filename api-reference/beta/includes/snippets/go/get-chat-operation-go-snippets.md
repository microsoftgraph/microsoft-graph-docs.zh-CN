---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cb060ebb960c0f540bd0fe27c88072862aa89d0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100185"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsAsyncOperationId := "teamsAsyncOperation-id"
result, err := graphClient.ChatsById(&chatId).OperationsById(&teamsAsyncOperationId).Get(options)


```