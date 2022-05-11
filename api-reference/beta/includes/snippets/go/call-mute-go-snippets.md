---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe015fe6d68956c6fb9cbc6bef9810b3d5c6d71a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327653"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClientContextRequestBody()
clientContext := "clientContext-value"
requestBody.SetClientContext(&clientContext)
callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).Mute(call-id).Post(requestBody)


```