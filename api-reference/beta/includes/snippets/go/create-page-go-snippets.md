---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 844dd08a1b958b82056f0ae75150dc453f4d2d0f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Pages().Post(requestBody)


```