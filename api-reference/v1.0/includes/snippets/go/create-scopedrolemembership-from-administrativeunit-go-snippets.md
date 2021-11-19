---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8135688e86ab4b72a42f3b04974b302f17c4369
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096819"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewScopedRoleMembership()
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
roleMemberInfo := msgraphsdk.NewIdentity()
requestBody.SetRoleMemberInfo(roleMemberInfo)
id := "id-value"
roleMemberInfo.SetId(&id)
options := &msgraphsdk.ScopedRoleMembersRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
result, err := graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).ScopedRoleMembers().Post(options)


```