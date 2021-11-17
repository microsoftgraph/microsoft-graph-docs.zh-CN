---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 676229904616f66ea437cb7790a8361a00941edf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019283"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

projectParticipationId := "projectParticipation-id"
result, err := graphClient.Me().Profile().ProjectsById(&projectParticipationId).Get(options)


```