---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d65d6559e192dcd501edab407210e3a60a6fe414
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033585"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
result, err := graphClient.TermStore().SetsById(&setId).Children().Get(options)


```