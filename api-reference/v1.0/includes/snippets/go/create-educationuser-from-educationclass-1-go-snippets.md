---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e232a37bc656cabf14f0edf91d58c3cd9418930e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097243"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/education/users/13015",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Members().$ref().Post(options)


```