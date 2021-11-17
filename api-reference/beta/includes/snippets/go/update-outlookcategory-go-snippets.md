---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3595fee3700cb723a80a99a612f30f1b95b79953
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018337"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOutlookCategory()
color := "preset15"
requestBody.SetColor(&color)
options := &msgraphsdk.OutlookCategoryRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookCategoryId := "outlookCategory-id"
graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Patch(options)


```