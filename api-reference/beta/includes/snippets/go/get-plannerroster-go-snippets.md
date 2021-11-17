---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac89e1183cfba9fdc804a62ef9f180c2f3db8cbd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021649"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerRosterId := "plannerRoster-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).Get(options)


```