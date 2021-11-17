---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4743063afc787040a9372c0e6bf13e89069d1800
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989210"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

teamId := "team-id"
timeCardId := "timeCard-id"
graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).Delete(options)


```