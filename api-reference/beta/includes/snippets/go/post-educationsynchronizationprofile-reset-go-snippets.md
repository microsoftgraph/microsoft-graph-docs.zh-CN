---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a35ab3a58635f98586ed6c3eb21eea5c5e4969c6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412043"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Reset(educationSynchronizationProfile-id).Post(nil)


```