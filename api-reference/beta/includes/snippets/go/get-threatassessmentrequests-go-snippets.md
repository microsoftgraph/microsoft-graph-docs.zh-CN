---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 783a885b6dd2f92e5fe38ea1b6d0e79c09ee8df4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327270"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Get()


```