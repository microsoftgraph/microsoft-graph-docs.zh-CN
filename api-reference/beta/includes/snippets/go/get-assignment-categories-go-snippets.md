---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5af3897df53fa8e044b955a1c5f5e969afe1d652
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Categories().Get(options)


```