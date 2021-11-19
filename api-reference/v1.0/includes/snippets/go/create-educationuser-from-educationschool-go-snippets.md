---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28188d3e7d90d91c34a6fe09e4913d5aa1307c17
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083114"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/education/users/14008",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
result, err := graphClient.Education().SchoolsById(&educationSchoolId).Users().$ref().Post(options)


```