---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef1fc894bb3989abb0596955fc9ecac518a696b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016056"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSubjectRightsRequest()
internalDueDateTime, err := time.Parse(time.RFC3339, "2021-08-30T00:00:00Z")
requestBody.SetInternalDueDateTime(&internalDueDateTime)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.subjectRightsRequest",
}
options := &msgraphsdk.SubjectRightsRequestRequestBuilderPatchOptions{
    Body: requestBody,
}
subjectRightsRequestId := "subjectRightsRequest-id"
graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Patch(options)


```