---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22ea4baeaee8b58fe94aa2dc12ab98a0e9dcbc45
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorGroupId := "connectorGroup-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroupsById(&connectorGroupId).Delete(options)


```