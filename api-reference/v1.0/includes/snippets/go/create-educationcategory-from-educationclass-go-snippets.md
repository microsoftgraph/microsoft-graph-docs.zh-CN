---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b7c038fd49fb9fcdbdd0de52ba23b7e4d6f6abc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326964"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationCategory()
displayName := "Quizzes"
requestBody.SetDisplayName(&displayName)
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategories().Post(requestBody)


```