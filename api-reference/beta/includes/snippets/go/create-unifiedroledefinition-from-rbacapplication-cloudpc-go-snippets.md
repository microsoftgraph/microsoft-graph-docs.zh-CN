---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27e8f6f66c8934b6f5831759beed91f17ed00abd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120033"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleDefinition()
description := "An example custom role"
requestBody.SetDescription(&description)
displayName := "ExampleCustomRole"
requestBody.SetDisplayName(&displayName)
requestBody.SetRolePermissions( []UnifiedRolePermission {
    msgraphsdk.NewUnifiedRolePermission(),
    SetAdditionalData(map[string]interface{}{
        "allowedResourceActions":  []String {
            "Microsoft.CloudPC/CloudPCs/Read",
        }
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "condition": "null",
}
options := &msgraphsdk.RoleDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().CloudPC().RoleDefinitions().Post(options)


```