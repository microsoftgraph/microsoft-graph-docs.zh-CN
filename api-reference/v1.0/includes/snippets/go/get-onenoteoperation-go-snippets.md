---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe3d79a7045c42afb60fd412faad70b153b97969
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033059"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onenoteOperationId := "onenoteOperation-id"
result, err := graphClient.Me().Onenote().OperationsById(&onenoteOperationId).Get(options)


```