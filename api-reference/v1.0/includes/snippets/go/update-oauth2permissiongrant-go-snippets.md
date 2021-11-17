---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60d9ad296e9843034517129680f1e99ca32c1d13
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996147"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
scope := "scope-value"
requestBody.SetScope(&scope)
options := &msgraphsdk.OAuth2PermissionGrantRequestBuilderPatchOptions{
    Body: requestBody,
}
oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Patch(options)


```