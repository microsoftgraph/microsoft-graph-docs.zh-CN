---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a126537603808d1fab90e062ac71b70901f5c4d5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationalActivityId := "educationalActivity-id"
result, err := graphClient.Me().Profile().EducationalActivitiesById(&educationalActivityId).Delete(nil)


```