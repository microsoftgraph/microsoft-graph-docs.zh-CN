---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2644809b72b86ab3129d02b619bfa8d7c23cce28
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088338"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
result, err := graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Get(options)


```