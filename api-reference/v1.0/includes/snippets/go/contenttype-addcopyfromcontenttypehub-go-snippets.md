---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9fc0ce020d2df7d79dd632f3a818c2a22302611
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315920"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentTypeIdRequestBody()
contentTypeId := "0x0101"
requestBody.SetContentTypeId(&contentTypeId)
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopyFromContentTypeHub(site-id, list-id).Post(requestBody)


```