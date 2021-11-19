---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5aaa6ed8d42c4c708c6169498e39640aa8caebce
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102525"
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
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).CopyToDefaultContentLocation().Post(options)


```