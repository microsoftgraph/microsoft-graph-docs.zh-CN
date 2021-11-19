---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c25b8c6563df3f833061b9337f24d3a70aafcbae
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091877"
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
options := &msgraphsdk.SubjectRightsRequestRequestBuilderPatchOptions{
    Body: requestBody,
}
subjectRightsRequestId := "subjectRightsRequest-id"
graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Patch(options)


```