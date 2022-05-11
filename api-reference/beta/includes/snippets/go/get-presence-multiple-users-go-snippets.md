---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2363877a61b6e26e35a9eba5b0ca2a90e17c4496
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328304"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdsRequestBody()
requestBody.SetIds( []String {
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b",
}
result, err := graphClient.Communications().GetPresencesByUserId().Post(requestBody)


```