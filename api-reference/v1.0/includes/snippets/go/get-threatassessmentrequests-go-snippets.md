---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32ae08f6bb5389f405d400e6412d4a382d0f8745
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Get(options)


```