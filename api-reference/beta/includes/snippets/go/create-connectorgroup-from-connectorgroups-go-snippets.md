---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59730514437b6f97a297e7748ab0779771ef3702
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026730"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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