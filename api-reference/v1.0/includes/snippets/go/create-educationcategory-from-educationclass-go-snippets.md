---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58bf9cd2399f7b5c3a8c505a642e41cb1d033aab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024666"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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