---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e7d0a8569db98dfb4135fdf326d560d9d28c785
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326404"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetQueryParameters{
    Expand: "inheritsPermissionsFrom",
}
options := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().Directory().RoleDefinitionsById(&unifiedRoleDefinitionId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```