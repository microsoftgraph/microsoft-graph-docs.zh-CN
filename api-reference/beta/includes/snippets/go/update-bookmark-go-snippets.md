---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c11e7b2988baab68bbd71f9749f36f9656dccc6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412661"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookmark()
description := "Book a fancy vacation in Tuscany or browse museums in Florence."
requestBody.SetDescription(&description)
options := &msgraphsdk.BookmarkRequestBuilderPatchOptions{
    Body: requestBody,
}
bookmarkId := "bookmark-id"
result, err := graphClient.Search().BookmarksById(&bookmarkId).Patch(options)


```