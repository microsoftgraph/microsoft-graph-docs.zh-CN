---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd8820d5442fd848d1aedd6317261b5295d88fb3
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759259"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOAuth2PermissionGrant()
scope := "User.ReadBasic.All Group.ReadWrite.All"
requestBody.SetScope(&scope)
options := &msgraphsdk.OAuth2PermissionGrantRequestBuilderPatchOptions{
    Body: requestBody,
}
oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Patch(options)


```