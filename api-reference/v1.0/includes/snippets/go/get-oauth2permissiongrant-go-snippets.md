---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aaafb47b9d0ac5a7c6f497c975a5eee53446164
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
result, err := graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Get(options)


```