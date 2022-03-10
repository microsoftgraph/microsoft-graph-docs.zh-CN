---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dbdabf80bcd738cf1be60a529d1544295f8b708
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412565"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationUser()
displayName := "Rogelio Cazares"
requestBody.SetDisplayName(&displayName)
givenName := "Rogelio"
requestBody.SetGivenName(&givenName)
middleName := "Fernando"
requestBody.SetMiddleName(&middleName)
surname := "Cazares"
requestBody.SetSurname(&surname)
options := &msgraphsdk.EducationUserRequestBuilderPatchOptions{
    Body: requestBody,
}
educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Patch(options)


```