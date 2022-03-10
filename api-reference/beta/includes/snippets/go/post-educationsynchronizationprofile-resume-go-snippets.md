---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65f1925cd64597c616580c87d12023e547fcbb9b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).Resume(educationSynchronizationProfile-id).Post(nil)


```