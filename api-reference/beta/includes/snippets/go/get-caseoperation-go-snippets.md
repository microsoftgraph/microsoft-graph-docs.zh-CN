---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46579c3588eb479eae25700d56f78f469cf01738
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
caseOperationId := "caseOperation-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).OperationsById(&caseOperationId).Get()


```