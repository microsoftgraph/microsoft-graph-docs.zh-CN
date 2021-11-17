---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c924760d46539b6344fddfde58e9faffa8f128f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993984"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
custodianId := "custodian-id"
unifiedGroupSourceId := "unifiedGroupSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSourcesById(&unifiedGroupSourceId).Delete(options)


```