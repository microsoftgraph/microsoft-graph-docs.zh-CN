---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd240a0de8b210ab9e125eb46d5d511bcb007b2a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327128"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationRubric()
displayName := "Example Credit Rubric after display name patch"
requestBody.SetDisplayName(&displayName)
educationRubricId := "educationRubric-id"
graphClient.Education().Me().RubricsById(&educationRubricId).Patch(requestBody)


```