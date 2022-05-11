---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac6d50a53101e12f1e9e3bf1a2864d5b644e163a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327143"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
longRunningOperationId := "longRunningOperation-id"
result, err := graphClient.UsersById(&userId).Authentication().OperationsById(&longRunningOperationId).Get()


```