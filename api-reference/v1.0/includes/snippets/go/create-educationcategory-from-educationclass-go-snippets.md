---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4048b29a44ef3dad5fc72709e3e8149675218122
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082094"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "displayName": "Quizzes",
}
options := &msgraphsdk.EducationCategoryRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationCategoryId := "educationCategory-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentCategoriesById(&educationCategoryId).Post(options)


```