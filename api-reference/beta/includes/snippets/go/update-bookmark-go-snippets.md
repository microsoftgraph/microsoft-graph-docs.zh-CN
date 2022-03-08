---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9c92d914188cd6c67895e4869410643da32bf5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338238"
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
graphClient.Search().BookmarksById(&bookmarkId).Patch(options)


```