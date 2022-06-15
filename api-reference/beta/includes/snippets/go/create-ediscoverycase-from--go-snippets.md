---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ac829af43f1b4d6ed33d1a5f67e8578a7201843
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095536"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryCase()
displayName := "CONTOSO LITIGATION-005"
requestBody.SetDisplayName(&displayName)
description := "Project Bazooka"
requestBody.SetDescription(&description)
externalId := "324516"
requestBody.SetExternalId(&externalId)
result, err := graphClient.Security().Cases().EdiscoveryCases().Post(requestBody)


```