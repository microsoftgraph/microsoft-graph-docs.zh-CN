---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0e275f22bb04ba25ff0b41a5699104eacea330a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).$value().Get(nil)


```