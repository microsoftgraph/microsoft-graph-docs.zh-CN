---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf31f57ae733a430338d7337f927ac56fee4e4b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412357"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personInterestId := "personInterest-id"
result, err := graphClient.Me().Profile().InterestsById(&personInterestId).Delete(nil)


```