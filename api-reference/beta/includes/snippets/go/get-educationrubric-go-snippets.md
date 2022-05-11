---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10e2255347f0d38d8fe2283600438d60b8d8b190
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329111"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationRubricId := "educationRubric-id"
result, err := graphClient.Education().Me().RubricsById(&educationRubricId).Get()


```