---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cde38870c02aec7ee684c500db8241fe3221a52
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976250"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

signInId := "signIn-id"
result, err := graphClient.AuditLogs().SignInsById(&signInId).Get(options)


```