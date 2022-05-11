---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 983beff7dd778cf77f285402a24e7767d73e5466
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
result, err := graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Get()


```