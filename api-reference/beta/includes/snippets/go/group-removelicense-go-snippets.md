---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b15abfca4c7c0fb265305feeef58fc54c8221cbe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAddLicenses( []AssignedLicense {
}
requestBody.SetRemoveLicenses( []String {
    "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "b05e124f-c7cc-45a0-a6aa-8cf78c946968",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).AssignLicense(group-id).Post(requestBody)


```