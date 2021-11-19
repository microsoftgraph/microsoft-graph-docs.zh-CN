---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82b8bd6cc00ba130fa625f49503094e49bd73724
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101059"
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
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Patch(options)


```