---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 748870be14d544d9880b16d19d39ea1f6581a349
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099633"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConnectorGroup()
name := "name-value"
requestBody.SetName(&name)
region := "region-value"
requestBody.SetRegion(&region)
options := &msgraphsdk.ConnectorGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorGroupId := "connectorGroup-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroupsById(&connectorGroupId).Patch(options)


```