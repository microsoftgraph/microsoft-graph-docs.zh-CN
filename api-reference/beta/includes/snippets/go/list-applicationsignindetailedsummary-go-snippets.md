---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dec1407ceea65d231d8f6059f4884e1a3bdd21e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327828"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Reports().ApplicationSignInDetailedSummary().Get()


```