---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4ab651d97e8e57dae2f2357f64c431565be63f3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327831"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
graphClient.ProgramsById(&programId).Delete()


```