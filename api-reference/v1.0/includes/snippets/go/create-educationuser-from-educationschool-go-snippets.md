---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eba5a800e4123db76efe11e17e2fac94612af366
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412700"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/education/users/14008",
}
options := &msgraphsdk.EducationUserRequestBuilderPostOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
educationUserId := "educationUser-id"
graphClient.Education().SchoolsById(&educationSchoolId).UsersById(&educationUserId).Post(options)


```