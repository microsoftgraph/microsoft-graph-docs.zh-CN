---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76e65c162b566245422690a8d9d1a15e83562ee1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979661"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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