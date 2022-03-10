---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33d9aed2bf3de9b59962da9cc344413fa3abb00b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personAwardId := "personAward-id"
result, err := graphClient.UsersById(&userId).Profile().AwardsById(&personAwardId).Delete(nil)


```