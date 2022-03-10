---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b54a1fcea8bbd94a4a8d3438f216d04b8c27e486
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412503"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
result, err := graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Start(educationSynchronizationProfile-id).Post(nil)


```