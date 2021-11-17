---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a683240eec24754a7e4440629ecf7cfc2cfba5a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023875"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Reopen().Post(options)


```