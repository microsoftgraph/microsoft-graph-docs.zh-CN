---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0376501faabcd083d3c30bbf7aca31fcae73207
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Delete(options)


```