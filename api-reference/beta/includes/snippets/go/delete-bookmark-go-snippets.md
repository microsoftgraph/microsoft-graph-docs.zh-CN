---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d69a31205fc2420f2b5a506c8008d86aa15a509e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338929"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

bookmarkId := "bookmark-id"
graphClient.Search().BookmarksById(&bookmarkId).Delete(nil)


```