---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a93c491af2fc5bca3aa08f4468b48bca940e384
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135119"
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
graphClient.Education().UsersById(&educationUserId).Patch(options)


```