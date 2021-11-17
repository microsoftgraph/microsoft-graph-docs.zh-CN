---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c0b3de7dd59924e89d99ba3190924fd8665e05
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019671"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
    Filter: "isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false",
}
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.PrivilegedRoleAssignments().Get(options)


```