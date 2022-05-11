---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5487d95d9a0bbfd490dc0ef63a63a6289d56f7b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328684"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGroupIdsRequestBody()
requestBody.SetGroupIds( []String {
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540",
}
result, err := graphClient.Me().CheckMemberGroups().Post(requestBody)


```