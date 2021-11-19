---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1991e0a153e7b06af5d45cdcb3e21bbdff10a2b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101484"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).History().Get(options)


```