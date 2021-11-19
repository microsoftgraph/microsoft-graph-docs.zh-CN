---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 208cb669ecf8a15ed05ae3172e9e2eb6cb2381a6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleDefinition()
description := "Update basic properties of application registrations"
requestBody.SetDescription(&description)
displayName := "Application Registration Support Administrator"
requestBody.SetDisplayName(&displayName)
requestBody.SetRolePermissions( []UnifiedRolePermission {
    msgraphsdk.NewUnifiedRolePermission(),
    SetAdditionalData(map[string]interface{}{
        "allowedResourceActions":  []String {
            "microsoft.directory/applications/basic/read",
        }
    }
}
isEnabled := "true"
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.RoleDefinitionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().Directory().RoleDefinitions().Post(options)


```