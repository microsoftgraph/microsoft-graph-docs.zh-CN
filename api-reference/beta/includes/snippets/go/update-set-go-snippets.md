---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7335e37197c6133f1daa71e368d7e9bfd2949363
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328828"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSet()
description := "mySet"
requestBody.SetDescription(&description)
setId := "set-id"
graphClient.TermStore().SetsById(&setId).Patch(requestBody)


```