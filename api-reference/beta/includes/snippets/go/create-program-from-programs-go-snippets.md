---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 353cc449e2eaa64480d0e878b03bd826b721d674
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315279"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProgram()
displayName := "testprogram3"
requestBody.SetDisplayName(&displayName)
description := "test description"
requestBody.SetDescription(&description)
result, err := graphClient.Programs().Post(requestBody)


```