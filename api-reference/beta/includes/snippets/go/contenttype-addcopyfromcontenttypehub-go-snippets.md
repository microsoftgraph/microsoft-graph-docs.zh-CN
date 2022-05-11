---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a28d2f1729a8a9199079347f5c547b92712d257
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentTypeIdRequestBody()
contentTypeId := "String"
requestBody.SetContentTypeId(&contentTypeId)
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopyFromContentTypeHub(site-id, list-id).Post(requestBody)


```