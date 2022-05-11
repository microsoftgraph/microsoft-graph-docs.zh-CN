---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f331f52f3d2cf4c5a8735d5461c52dccff8fff97
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328980"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().ActivityBasedTimeoutPolicies().Get()


```