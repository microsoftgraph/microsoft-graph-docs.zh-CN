---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb4e2b09d5cf59e7cf0455b8ebcb31cd9d8c378
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412264"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
custodianId := "custodian-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).Activate(case-id, custodian-id).Post(nil)


```