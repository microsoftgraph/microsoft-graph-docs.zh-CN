---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c88e2e46809b45f518a60fbf18c7e9c2dc6e91b7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976517"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.InformationProtection().ThreatAssessmentRequests().Get(options)


```