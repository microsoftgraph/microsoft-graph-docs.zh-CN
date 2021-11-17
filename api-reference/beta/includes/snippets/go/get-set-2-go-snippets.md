---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4afaae57ff4a19a7f6f7a87b1d5a6d30a2ef826b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017414"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Get(options)


```