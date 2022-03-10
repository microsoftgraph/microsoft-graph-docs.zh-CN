---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b4f0192ea0b27bcd7f3d65090b3eda8ed68347f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412421"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Pause(educationSynchronizationProfile-id).Post(nil)


```