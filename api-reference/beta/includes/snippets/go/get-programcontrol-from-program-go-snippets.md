---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b379e5f9e9f55bf129e296075164df4962c7e45c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314185"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
result, err := graphClient.ProgramsById(&programId).Controls().Get()


```