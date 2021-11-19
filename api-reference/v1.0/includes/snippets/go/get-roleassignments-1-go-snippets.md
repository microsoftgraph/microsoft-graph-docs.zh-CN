---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84e3072ad0dc55b8a4258ac0e0b4491217422867
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091664"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "roleDefinitionId%20eq%20'62e90394-69f5-4237-9190-012177145e10'",
    Expand: "principal",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().Get(options)


```