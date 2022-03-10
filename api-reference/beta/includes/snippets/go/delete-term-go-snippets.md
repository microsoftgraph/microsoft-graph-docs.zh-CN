---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf540bfa1ced60f61f8d969330444ca74d00d469
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

setId := "set-id"
termId := "term-id"
result, err := graphClient.TermStore().SetsById(&setId).TermsById(&termId).Delete(nil)


```