---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 106d13d0497cc48c8955e153135575e08b49dbab
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

signInId := "signIn-id"
result, err := graphClient.AuditLogs().SignInsById(&signInId).Get(options)


```