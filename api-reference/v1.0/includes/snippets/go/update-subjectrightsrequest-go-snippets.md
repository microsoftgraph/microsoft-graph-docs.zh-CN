---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 714c3599e6efc56510ee97ea5217bac4d1f5e501
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325974"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSubjectRightsRequest()
internalDueDateTime, err := time.Parse(time.RFC3339, "2021-08-30T00:00:00Z")
requestBody.SetInternalDueDateTime(&internalDueDateTime)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.subjectRightsRequest",
}
subjectRightsRequestId := "subjectRightsRequest-id"
graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Patch(requestBody)


```