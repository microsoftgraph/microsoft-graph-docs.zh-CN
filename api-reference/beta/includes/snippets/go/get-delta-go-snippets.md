---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: deb79687d889480fea54766eae5d37bc99c104a1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989965"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerDeltaId := "plannerDelta-id"
result, err := graphClient.Me().Planner().AllById(&plannerDeltaId).Get(options)


```