---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2570ee4eb07ddaad8431eee6fb7ffe354f7cca4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032100"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onenoteResourceId := "onenoteResource-id"
graphClient.Me().Onenote().ResourcesById(&onenoteResourceId).Content().Get(options)


```