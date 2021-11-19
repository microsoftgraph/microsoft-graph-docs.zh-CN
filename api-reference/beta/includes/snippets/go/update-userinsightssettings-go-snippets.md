---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b8bee09ca7622d63b45f8ad0bbcfd32583e5c1a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097764"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserInsightsSettings()
isEnabled := "false"
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.ItemInsightsRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Settings().ItemInsights().Patch(options)


```