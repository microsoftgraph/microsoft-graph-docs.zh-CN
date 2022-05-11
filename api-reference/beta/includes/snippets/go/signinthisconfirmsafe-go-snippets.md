---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a2d243b6a5b99a5fed0ddf7713d85d6cc096b14
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326367"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRequestIdsRequestBody()
requestBody.SetRequestIds( []String {
    "5a0c76d2-cb57-4ece-9bc1-c323178f116a",
    "96609214-09ef-4f80-9d4a-ace5fceecaec",
    "05020696-4eb8-45a3-918f-8f8bb7ad6015",
}
graphClient.AuditLogs().SignIns().ConfirmSafe().Post(requestBody)


```