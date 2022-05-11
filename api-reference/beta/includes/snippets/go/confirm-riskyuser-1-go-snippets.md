---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d07fc2861427103a9dd1fc160a8d918dad2c8dd4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329083"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserIdsRequestBody()
requestBody.SetUserIds( []String {
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471",
}
graphClient.RiskyUsers().ConfirmCompromised().Post(requestBody)


```