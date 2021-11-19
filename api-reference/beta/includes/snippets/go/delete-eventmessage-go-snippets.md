---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1de3c712256e897717da265b5377e3ae92b1857
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093125"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Delete(options)


```