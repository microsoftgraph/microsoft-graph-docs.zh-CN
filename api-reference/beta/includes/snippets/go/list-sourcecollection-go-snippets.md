---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfa182c952ec82b563ee5400ba36fe409df43d22
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032626"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollections().Get(options)


```