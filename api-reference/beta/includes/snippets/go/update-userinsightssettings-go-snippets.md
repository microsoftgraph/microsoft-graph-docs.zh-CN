---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 516c3d27e31835a58da8b73a4f910126a91d3106
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328120"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserInsightsSettings()
isEnabled := "false"
requestBody.SetIsEnabled(&isEnabled)
userId := "user-id"
graphClient.UsersById(&userId).Settings().ItemInsights().Patch(requestBody)


```