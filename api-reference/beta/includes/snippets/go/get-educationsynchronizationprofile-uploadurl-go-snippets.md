---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 747d4278c3c3c2ceffee2204b2c26c9eaff947f6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationSynchronizationProfileId := "educationSynchronizationProfile-id"
result, err := graphClient.Education().SynchronizationProfilesById(&educationSynchronizationProfileId).UploadUrl()(educationSynchronizationProfile-id).Get(nil)


```