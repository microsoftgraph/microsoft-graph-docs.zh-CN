---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 437d98ecab886cb1ed936b10cbb0d3be4011b082
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
riskyUserHistoryItemId := "riskyUserHistoryItem-id"
result, err := graphClient.IdentityProtection().RiskyUsersById(&riskyUserId).HistoryById(&riskyUserHistoryItemId).Get(nil)


```