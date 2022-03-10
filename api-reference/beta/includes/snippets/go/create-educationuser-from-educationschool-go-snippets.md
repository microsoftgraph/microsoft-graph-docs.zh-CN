---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1172ac9b6f62d24d91d307cf04853bfaa0eaceaa
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/education/users/14008",
}
options := &msgraphsdk.EducationUserRequestBuilderPostOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
educationUserId := "educationUser-id"
graphClient.Education().SchoolsById(&educationSchoolId).UsersById(&educationUserId).Post(options)


```