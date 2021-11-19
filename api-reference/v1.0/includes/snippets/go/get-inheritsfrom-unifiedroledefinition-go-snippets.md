---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dfad6ea0d38ce4c2abcce3cbcbad01f2f6fcce8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetQueryParameters{
    Expand: "inheritsPermissionsFrom",
}
options := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetOptions{
    Q: requestParameters,
}
unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).Get(options)


```