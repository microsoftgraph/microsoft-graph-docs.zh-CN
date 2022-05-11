---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98c8bf8c631e137b7cb3c446b5c1991404deb1ce
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328556"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
reason := "busy"
requestBody.SetReason(&reason)
callId := "call-id"
graphClient.Communications().CallsById(&callId).Reject(call-id).Post(requestBody)


```