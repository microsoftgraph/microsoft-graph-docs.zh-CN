---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c27cd5f640465037cfab575ce050f901f22d504
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328137"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Delete()


```