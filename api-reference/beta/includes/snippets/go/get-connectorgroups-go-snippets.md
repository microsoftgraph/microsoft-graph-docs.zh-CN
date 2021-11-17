---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b54144146d66f325b55b7ed7954f0806f843856
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024952"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroups().Get(options)


```