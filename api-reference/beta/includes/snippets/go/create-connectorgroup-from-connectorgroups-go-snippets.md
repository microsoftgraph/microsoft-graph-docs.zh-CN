---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 012c01a3fb1f531a470ca02000609d44e534aea3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087866"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConnectorGroup()
name := "name-value"
requestBody.SetName(&name)
isDefault := false
requestBody.SetIsDefault(&isDefault)
options := &msgraphsdk.ConnectorGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroups().Post(options)


```