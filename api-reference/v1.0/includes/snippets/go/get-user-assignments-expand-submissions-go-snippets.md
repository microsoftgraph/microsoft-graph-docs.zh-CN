---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5c659277543c6d4a6eafef4a7dbc5986af8ad19
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AssignmentsRequestBuilderGetQueryParameters{
    Expand: "submissions",
}
options := &msgraphsdk.AssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Assignments().Get(options)


```