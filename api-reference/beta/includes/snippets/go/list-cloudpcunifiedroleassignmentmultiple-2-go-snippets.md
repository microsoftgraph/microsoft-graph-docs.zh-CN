---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd0cb59edf05b8d7ad0046256d1da1627e8091f7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090555"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "roleDefinitionId%20eq%20'b5c08161-a7af-481c-ace2-a20a69a48fb1'",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().CloudPC().RoleAssignments().Get(options)


```