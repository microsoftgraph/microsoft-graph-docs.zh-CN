---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43be92550c4d34ffb3a7d0b4d98553ee8500c71e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099863"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
tenantGroupId := "String"
requestBody.SetTenantGroupId(&tenantGroupId)
tenantId := "String"
requestBody.SetTenantId(&tenantId)
managementActionId := "String"
requestBody.SetManagementActionId(&managementActionId)
managementTemplateId := "String"
requestBody.SetManagementTemplateId(&managementTemplateId)
status := "String"
requestBody.SetStatus(&status)
options := &msgraphsdk.ChangeDeploymentStatusRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementActionTenantDeploymentStatuses().ChangeDeploymentStatus().Post(options)


```