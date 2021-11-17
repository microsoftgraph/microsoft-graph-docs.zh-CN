---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3077be1be7fea5af3493b871ffa92d0e3b9068c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986620"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AssignmentsRequestBuilderGetQueryParameters{
    Expand: "resources",
}
options := &msgraphsdk.AssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().Get(options)


```