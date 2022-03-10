---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e96be5a4576c7b91d752509a697a932f82a3a8a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412514"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOutlookCategory()
color := "preset15"
requestBody.SetColor(&color)
options := &msgraphsdk.OutlookCategoryRequestBuilderPatchOptions{
    Body: requestBody,
}
outlookCategoryId := "outlookCategory-id"
result, err := graphClient.Me().Outlook().MasterCategoriesById(&outlookCategoryId).Patch(options)


```