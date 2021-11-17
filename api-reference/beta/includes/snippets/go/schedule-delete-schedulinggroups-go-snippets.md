---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07dc530c430785bae1898b4485110b0f2e03454e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020578"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Delete(options)


```