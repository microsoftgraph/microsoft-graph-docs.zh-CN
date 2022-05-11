---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 796cb55f703db4373fd7d67bed9b16d3c0285830
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328614"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentTypeRequestBody()
contentType := "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
requestBody.SetContentType(&contentType)
siteId := "site-id"
listId := "list-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ContentTypes().AddCopy(site-id, list-id).Post(requestBody)


```