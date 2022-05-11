---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e11a72fc6a52f13ee9d6dde74ab8146c14e4c3c0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328148"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProgram()
displayName := "testprogram3 new name"
requestBody.SetDisplayName(&displayName)
programId := "program-id"
graphClient.ProgramsById(&programId).Patch(requestBody)


```