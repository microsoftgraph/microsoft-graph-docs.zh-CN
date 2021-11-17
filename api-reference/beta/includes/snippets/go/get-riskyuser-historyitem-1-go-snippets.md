---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ea63c14c829a2485ca880a947b7ad737f76ef3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002741"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

riskyUserId := "riskyUser-id"
riskyUserHistoryItemId := "riskyUserHistoryItem-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).HistoryById(&riskyUserHistoryItemId).Get(options)


```