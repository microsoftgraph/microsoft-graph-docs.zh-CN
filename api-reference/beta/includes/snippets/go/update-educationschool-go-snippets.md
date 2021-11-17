---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce65906e1fb266bf00adf62401ef948aec19cb9f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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