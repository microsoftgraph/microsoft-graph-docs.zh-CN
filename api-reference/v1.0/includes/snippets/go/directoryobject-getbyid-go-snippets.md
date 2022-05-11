---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afac035b803844f115647f9a31bb56aa8df0394c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326434"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "84b80893874940a3-97b7-68513b600544",
    "5d6059b6368d-45f8-91e18e07d485f1d0",
}
requestBody.SetTypes( []String {
    "user",
}
result, err := graphClient.DirectoryObjects().GetByIds().Post(requestBody)


```