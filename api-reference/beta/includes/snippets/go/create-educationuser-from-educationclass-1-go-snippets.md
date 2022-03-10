---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9fb31b3a6410de85b74dd25b22922b9506c1883
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412631"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/education/users/13015",
}
options := &msgraphsdk.EducationUserRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationUserId := "educationUser-id"
graphClient.Education().ClassesById(&educationClassId).MembersById(&educationUserId).Post(options)


```