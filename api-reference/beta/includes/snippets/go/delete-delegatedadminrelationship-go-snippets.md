---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b6df01c27ed7f9d68a820af2ecac039a37e5ac9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202417"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "If-Match": "W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==""
}
options := &msgraphsdk.DelegatedAdminRelationshipRequestBuilderDeleteOptions{
    H: headers,
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).Delete(options)


```