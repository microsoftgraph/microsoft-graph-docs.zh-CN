---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34391c90c084c91ccb55878cdb530dce1fe48b96
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210298"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "If-Match": "W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==""
}
options := &msgraphsdk.DelegatedAdminAccessAssignmentRequestBuilderDeleteOptions{
    H: headers,
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminAccessAssignmentId := "delegatedAdminAccessAssignment-id"
graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).AccessAssignmentsById(&delegatedAdminAccessAssignmentId).Delete(options)


```