---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 917332b4c05473b6fc88c76470872da82500fc65
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327487"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
reason := "none"
requestBody.SetReason(&reason)
callId := "call-id"
graphClient.Communications().CallsById(&callId).Reject(call-id).Post(requestBody)


```