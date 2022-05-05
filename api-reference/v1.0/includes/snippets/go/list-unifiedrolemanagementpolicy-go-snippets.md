---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf78e81e1c41461f10fcdfed346491ee2acb5d0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207648"
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