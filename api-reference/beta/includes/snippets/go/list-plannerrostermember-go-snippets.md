---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b18d4bb856a113dc3cb43cad254406a8ce15970
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).Members().Get(options)


```