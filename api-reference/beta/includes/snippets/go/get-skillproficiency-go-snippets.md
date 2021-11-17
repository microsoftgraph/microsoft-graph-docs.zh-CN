---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bca2c159565e6d24451f507f9220e38525c3470
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031807"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

skillProficiencyId := "skillProficiency-id"
result, err := graphClient.Me().Profile().SkillsById(&skillProficiencyId).Get(options)


```