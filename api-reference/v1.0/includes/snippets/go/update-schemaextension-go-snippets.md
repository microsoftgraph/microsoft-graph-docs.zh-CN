---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e77efd86c7e7ce7d9009ac79b68f7a2cd20a2ec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326491"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
requestBody.SetAdditionalData(map[string]interface{}{
}
userId := "user-id"
graphClient.UsersById(&userId).Patch(requestBody)


```