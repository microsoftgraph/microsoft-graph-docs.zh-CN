---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 278391ae30144cce3a9ff5b0af90ba50cad4499e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328561"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

workPositionId := "workPosition-id"
result, err := graphClient.Me().Profile().PositionsById(&workPositionId).Get()


```