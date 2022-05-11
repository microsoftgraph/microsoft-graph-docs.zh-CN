---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd811f82eaca2ff1184cbd114b720e48f4596b27
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRequestIdsRequestBody()
requestBody.SetRequestIds( []String {
    "f01c6af6-6683-4a37-a945-0a925501eede",
    "42bf60ac-d0cb-4206-aa5c-101884298f55",
    "f09c8f14-8d8e-42cf-8a7e-732b0594e79b",
}
graphClient.AuditLogs().SignIns().ConfirmCompromised().Post(requestBody)


```