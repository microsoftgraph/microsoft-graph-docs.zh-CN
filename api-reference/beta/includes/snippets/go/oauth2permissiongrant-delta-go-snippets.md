---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1018a1751ba93afecc42b14bdc059893848f5849
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
result, err := graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Get(options)


```