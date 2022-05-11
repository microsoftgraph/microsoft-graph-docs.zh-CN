---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a4f8016b15b5522b424ee4d1360c1301c034f07
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326965"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).TaughtClasses().Get()


```