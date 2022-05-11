---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 264d372b08bc96090d7633957620e79b4f1daaaa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327985"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/education/classes/11006",
}
educationSchoolId := "educationSchool-id"
educationClassId := "educationClass-id"
graphClient.Education().SchoolsById(&educationSchoolId).ClassesById(&educationClassId).Post(requestBody)


```