---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d5dec1d418342c30d0e3f435c3864b0d7edfed4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008533"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetQueryParameters{
    Expand: "inheritsPermissionsFrom",
}
options := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```