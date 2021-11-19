---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd543f60cd0e513cf204a7c02f295758bbcfca31
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

projectParticipationId := "projectParticipation-id"
result, err := graphClient.Me().Profile().ProjectsById(&projectParticipationId).Get(options)


```