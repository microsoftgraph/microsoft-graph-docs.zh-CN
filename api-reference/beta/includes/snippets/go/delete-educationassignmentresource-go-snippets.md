---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d96d85bc7ce94175b226d801230808605c778ea
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationAssignmentResourceId := "educationAssignmentResource-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).ResourcesById(&educationAssignmentResourceId).Delete(options)


```