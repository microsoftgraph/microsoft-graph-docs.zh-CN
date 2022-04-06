---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf78e81e1c41461f10fcdfed346491ee2acb5d0
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759160"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetQueryParameters{
    Filter: "scopeId%20eq%20'/'%20and%20scopeType%20eq%20'DirectoryRole'",
}
options := &msgraphsdk.RoleManagementPoliciesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Policies().RoleManagementPolicies().Get(options)


```