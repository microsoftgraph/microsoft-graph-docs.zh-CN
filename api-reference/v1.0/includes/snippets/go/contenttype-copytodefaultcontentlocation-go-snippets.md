---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fca0333f70f9eac711b5895cde226499108e3f98
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974186"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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