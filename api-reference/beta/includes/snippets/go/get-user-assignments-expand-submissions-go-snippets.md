---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5c659277543c6d4a6eafef4a7dbc5986af8ad19
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086457"
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