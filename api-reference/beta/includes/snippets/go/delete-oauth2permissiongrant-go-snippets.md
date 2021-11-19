---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88658507d90b0d38c10f53bd5f2201af4ec08bbd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083974"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Delete(options)


```