---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26b69969f440a74e750b0a36bfcf9137fa45c586
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022342"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
custodianId := "custodian-id"
siteSourceId := "siteSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).SiteSourcesById(&siteSourceId).Delete(options)


```