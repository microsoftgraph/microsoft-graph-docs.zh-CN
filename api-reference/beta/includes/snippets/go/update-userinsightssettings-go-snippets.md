---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11f726ea2caa024ea57225c70726aec9c499e3a9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUserInsightsSettings()
isEnabled := "false"
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.ItemInsightsRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Settings().ItemInsights().Patch(options)


```