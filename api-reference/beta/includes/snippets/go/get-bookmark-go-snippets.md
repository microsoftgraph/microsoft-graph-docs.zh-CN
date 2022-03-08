---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af4cac46501385673657f826a51d20136d1ab6f3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338311"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookmarkId := "bookmark-id"
result, err := graphClient.Search().BookmarksById(&bookmarkId).Get(nil)


```