---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d1fca668aec7521923622fe1f73e2a4ada3838d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

workPositionId := "workPosition-id"
result, err := graphClient.Me().Profile().PositionsById(&workPositionId).Delete(nil)


```