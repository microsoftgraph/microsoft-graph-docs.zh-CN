---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b77a3f13659c89cafc71ec6d5aca4afb7da98541
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412675"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

languageProficiencyId := "languageProficiency-id"
result, err := graphClient.Me().Profile().LanguagesById(&languageProficiencyId).Delete(nil)


```