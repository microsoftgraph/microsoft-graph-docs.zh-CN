---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2f22b3a163e16938872aa1b245c9bf5b66dd8b5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091658"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
result, err := graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Get(options)


```