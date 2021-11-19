---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 157d7e217cfb6ac125a54fe630198a9ec02f44f5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097161"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskyUserId := "riskyUser-id"
result, err := graphClient.RiskyUsersById(&riskyUserId).Get(options)


```