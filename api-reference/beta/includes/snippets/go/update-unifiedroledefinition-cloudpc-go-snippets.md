---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a9af1de7af49d3ff5bded001c9a9d62eed5dfb4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089123"
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
graphClient.RoleManagement().CloudPC().RoleDefinitionsById(&unifiedRoleDefinitionId).Patch(options)


```