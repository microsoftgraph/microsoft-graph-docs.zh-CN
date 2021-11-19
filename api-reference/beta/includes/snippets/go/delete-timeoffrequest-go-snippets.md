---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7af38a553e147b5b444b7cc1cb8af12ef0e98351
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102899"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
timeOffRequestId := "timeOffRequest-id"
graphClient.TeamsById(&teamId).Schedule().TimeOffRequestsById(&timeOffRequestId).Delete(options)


```