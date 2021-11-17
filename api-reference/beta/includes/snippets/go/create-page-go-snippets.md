---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9804f69a66818735b389f768c8bf056c203a625b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSitePage()
name := "Events.aspx"
requestBody.SetName(&name)
title := "Team Events"
requestBody.SetTitle(&title)
publishingState := msgraphsdk.NewPublicationFacet()
requestBody.SetPublishingState(publishingState)
level := "checkedOut"
publishingState.SetLevel(&level)
versionId := "0.1"
publishingState.SetVersionId(&versionId)
requestBody.SetWebParts( []WebPart {
    msgraphsdk.NewWebPart(),
    SetAdditionalData(map[string]interface{}{
        "type": "rte",
    }
    msgraphsdk.NewWebPart(),
    SetAdditionalData(map[string]interface{}{
        "type": "d1d91016-032f-456d-98a4-721247c305e8",
    }
}
options := &msgraphsdk.PagesRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Pages().Post(options)


```