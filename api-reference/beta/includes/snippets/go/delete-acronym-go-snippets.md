---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a094abc93677926858c66a3ace440cca2f92281
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

acronymId := "acronym-id"
graphClient.Search().AcronymsById(&acronymId).Delete()


```