---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae4e363da7d57c4bc3846104076f52adffba099e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023210"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
openShiftId := "openShift-id"
graphClient.TeamsById(&teamId).Schedule().OpenShiftsById(&openShiftId).Delete(options)


```