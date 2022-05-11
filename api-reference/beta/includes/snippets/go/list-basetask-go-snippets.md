---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a9490caff4069404793652f2f9910bfe5e4ea9b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326396"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).Tasks().Get()


```