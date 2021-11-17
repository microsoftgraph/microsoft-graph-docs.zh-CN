---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a93cad4f3325f040220d1701457a47865a25ca8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019206"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

workPositionId := "workPosition-id"
result, err := graphClient.Me().Profile().PositionsById(&workPositionId).Get(options)


```