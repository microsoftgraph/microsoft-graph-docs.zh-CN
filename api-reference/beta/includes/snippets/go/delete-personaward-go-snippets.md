---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9677966c9db5e633c8add0126b74ae21ae7c836
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086367"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
personAwardId := "personAward-id"
graphClient.UsersById(&userId).Profile().AwardsById(&personAwardId).Delete(options)


```