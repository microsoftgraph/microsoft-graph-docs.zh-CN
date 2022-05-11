---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b720addfc45f6358c6ad7b27b6a695ab1c7f840
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328616"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContactMergeSuggestions()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
graphClient.Me().Settings().ContactMergeSuggestions().Patch(requestBody)


```