---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3202662084471de0d63b4141a519a21931397b64
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326658"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

skillProficiencyId := "skillProficiency-id"
result, err := graphClient.Me().Profile().SkillsById(&skillProficiencyId).Get()


```