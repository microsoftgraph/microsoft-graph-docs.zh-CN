---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 859a4cc84799acae5e12b0f06ec314c9ff2e81ed
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975313"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Delete(options)


```