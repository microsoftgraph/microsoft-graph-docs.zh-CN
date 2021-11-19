---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 353661158e455694bc9c07c9c02b1f756af40ea0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086397"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).Delete(options)


```