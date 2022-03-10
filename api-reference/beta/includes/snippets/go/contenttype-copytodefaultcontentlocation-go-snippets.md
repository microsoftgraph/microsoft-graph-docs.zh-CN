---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdd4d4b7dab2fe70e898e1641acdef61ae222f0e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411768"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
sourceFile := msgraphsdk.NewItemReference()
requestBody.SetSourceFile(sourceFile)
sharepointIds := msgraphsdk.NewSharepointIds()
sourceFile.SetSharepointIds(sharepointIds)
listId := "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0"
sharepointIds.SetListId(&listId)
listItemId := "2"
sharepointIds.SetListItemId(&listItemId)
destinationFileName := "newname.txt"
requestBody.SetDestinationFileName(&destinationFileName)
options := &msgraphsdk.CopyToDefaultContentLocationRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).CopyToDefaultContentLocation(site-id, contentType-id).Post(options)


```