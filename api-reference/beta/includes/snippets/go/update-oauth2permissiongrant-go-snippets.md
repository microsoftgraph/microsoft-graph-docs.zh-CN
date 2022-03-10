---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 926ee5650dd8c3a8ac4da0536cb01e37e04b456f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
scope := "scope-value"
requestBody.SetScope(&scope)
options := &msgraphsdk.OAuth2PermissionGrantRequestBuilderPatchOptions{
    Body: requestBody,
}
oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
result, err := graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Patch(options)


```