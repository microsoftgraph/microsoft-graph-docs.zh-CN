---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5be40dea0c639bca6a2b6b30aaec5ffee60e074
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411816"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
type := "embed"
requestBody.SetType(&type)
options := &msgraphsdk.CreateLinkRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).CreateLink(site-id, list-id, listItem-id).Post(options)


```