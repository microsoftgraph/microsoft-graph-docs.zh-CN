---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c350f5d6a6c265d1468dd8894c7f6d966126479e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098612"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

riskDetectionId := "riskDetection-id"
result, err := graphClient.IdentityProtection().RiskDetectionsById(&riskDetectionId).Get(options)


```