---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5afea3d7d9a94cbf74c7e24dc06a2d856343401
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019672"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().Get(options)


```