---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bf9b313a06713dce4b866c79130162f9a413e13
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCase()
displayName := "My Case 1"
requestBody.SetDisplayName(&displayName)
result, err := graphClient.Compliance().Ediscovery().Cases().Post(requestBody)


```