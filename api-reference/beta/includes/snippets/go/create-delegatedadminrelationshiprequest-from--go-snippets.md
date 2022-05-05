---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c62f99200398db79048dd7fc89dcd4f7e09227e8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203470"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminRelationshipRequest()
action := "lockForApproval"
requestBody.SetAction(&action)
options := &msgraphsdk.RequestsRequestBuilderPostOptions{
    Body: requestBody,
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).Requests().Post(options)


```