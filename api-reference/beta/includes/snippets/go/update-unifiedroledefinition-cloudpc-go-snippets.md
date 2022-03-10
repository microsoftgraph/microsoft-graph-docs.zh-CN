---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d92e58989bb4b328f3b7def0319be449ef97a9b7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412340"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleDefinition()
description := "Update basic properties and permission of application registrations"
requestBody.SetDescription(&description)
displayName := "ExampleCustomRole"
requestBody.SetDisplayName(&displayName)
requestBody.SetRolePermissions( []UnifiedRolePermission {
    msgraphsdk.NewUnifiedRolePermission(),
    SetAdditionalData(map[string]interface{}{
        "allowedResourceActions":  []String {
            "Microsoft.CloudPC/CloudPCs/Read",
            "Microsoft.CloudPC/CloudPCs/Reprovision",
        }
    }
}
options := &msgraphsdk.UnifiedRoleDefinitionRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleDefinitionId := "unifiedRoleDefinition-id"
result, err := graphClient.RoleManagement().CloudPC().RoleDefinitionsById(&unifiedRoleDefinitionId).Patch(options)


```