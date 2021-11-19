---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5622891ac6f460d8335a39619a296ee119100a48
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100714"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
legalHoldId := "legalHold-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).Delete(options)


```