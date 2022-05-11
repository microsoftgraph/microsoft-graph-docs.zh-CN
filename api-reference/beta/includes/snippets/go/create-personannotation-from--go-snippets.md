---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ba85efb2454f05b6eac459817dbb68e8e2aef99
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnotation()
detail := msgraphsdk.NewItemBody()
requestBody.SetDetail(detail)
contentType := "text"
detail.SetContentType(&contentType)
content := "I am originally from Australia, but grew up in Moscow, Russia."
detail.SetContent(&content)
displayName := "About Me"
requestBody.SetDisplayName(&displayName)
result, err := graphClient.Me().Profile().Notes().Post(requestBody)


```