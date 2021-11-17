---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ac34d4b09eb297d60436b3119ba46dd82dcda10
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985331"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Me().Planner().Tasks().Get(options)


```