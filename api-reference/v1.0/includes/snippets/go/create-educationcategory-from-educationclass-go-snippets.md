---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c16661101013b1761379c43bc2b6993328095a4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136278"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationCategory()
displayName := "Quizzes"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AssignmentCategoriesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentCategories().Post(options)


```