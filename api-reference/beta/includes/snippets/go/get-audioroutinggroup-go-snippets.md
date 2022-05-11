---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f28aa0cf5c9067287319c88db994fb9492a825c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326488"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Get()


```