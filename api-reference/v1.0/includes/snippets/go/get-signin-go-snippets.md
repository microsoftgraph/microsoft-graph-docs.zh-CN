---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2f6436885e2b4a75a84aa2baadd1a891b6ad51
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

signInId := "signIn-id"
result, err := graphClient.AuditLogs().SignInsById(&signInId).Get()


```