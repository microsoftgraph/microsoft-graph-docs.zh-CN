---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 899a09e4179829cbba6f3556b02c418c146139fa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326679"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookCategory()
displayName := "Project expenses"
requestBody.SetDisplayName(&displayName)
color := "preset9"
requestBody.SetColor(&color)
result, err := graphClient.Me().Outlook().MasterCategories().Post(requestBody)


```