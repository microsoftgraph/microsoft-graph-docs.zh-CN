---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0fc89c30fbef827eb5fef717bbf2dd272bceb8b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationCategory()
displayName := "Quizzes"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AssignmentCategoriesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategories().Post(options)


```