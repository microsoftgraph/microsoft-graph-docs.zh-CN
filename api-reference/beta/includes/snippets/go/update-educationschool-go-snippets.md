---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4f83423a4ea52c12d98d8951eb8dbff958737d0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092428"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSchool()
displayName := "Fabrikam Arts High School"
requestBody.SetDisplayName(&displayName)
description := "Magnate school for the arts. Los Angeles School District"
requestBody.SetDescription(&description)
options := &msgraphsdk.EducationSchoolRequestBuilderPatchOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
graphClient.Education().SchoolsById(&educationSchoolId).Patch(options)


```