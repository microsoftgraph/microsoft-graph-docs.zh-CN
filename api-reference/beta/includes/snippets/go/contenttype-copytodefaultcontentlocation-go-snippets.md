---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f54932f5ed5b85b0e92f43f52483d4b6f8db6e92
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327474"
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
siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).CopyToDefaultContentLocation(site-id, contentType-id).Post(requestBody)


```