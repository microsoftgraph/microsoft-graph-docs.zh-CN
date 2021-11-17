---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5df414d5ae189d3242b86c3e5cd11253e6202e8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979577"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().AuthenticationFlowsPolicy().Get(options)


```