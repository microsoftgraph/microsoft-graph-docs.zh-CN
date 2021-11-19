---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 072200b39e9d4024ed3222f0d845980270449d1e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorId := "connector-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorsById(&connectorId).MemberOf().Get(options)


```