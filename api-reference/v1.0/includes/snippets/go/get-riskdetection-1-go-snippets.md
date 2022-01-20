---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 048bf4529ab50b9d3008e1b0059ad25e16b4bc50
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088234"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskDetectionId := "riskDetection-id"
result, err := graphClient.IdentityProtection().RiskDetectionsById(&riskDetectionId).Get(nil)


```