---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbde69fde256e407d4f741a2bd1f0bf4b53b9d48
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032584"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
custodianId := "custodian-id"
unifiedGroupSourceId := "unifiedGroupSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSourcesById(&unifiedGroupSourceId).Get(options)


```