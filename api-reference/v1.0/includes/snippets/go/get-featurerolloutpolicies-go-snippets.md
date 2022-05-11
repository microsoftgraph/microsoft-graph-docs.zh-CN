---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fc02e3f31367f5c34b1d0596bb3f19ccbc80a5f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().FeatureRolloutPolicies().Get()


```