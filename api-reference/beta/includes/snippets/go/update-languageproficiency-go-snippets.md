---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20e7e556d5a191b90d68e1445950f1097968dbea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewLanguageProficiency()
allowedAudiences := "organization"
requestBody.SetAllowedAudiences(&allowedAudiences)
languageProficiencyId := "languageProficiency-id"
graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Patch(requestBody)


```