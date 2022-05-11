---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9eca1d1e9b478bbd103229144950bdbf47ff7e97
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPasswordRequestBody()
password := "1234567890"
requestBody.SetPassword(&password)
result, err := graphClient.Users().ValidatePassword().Post(requestBody)


```