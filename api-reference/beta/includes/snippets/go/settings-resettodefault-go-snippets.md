---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ff9e09bae9d9a7e6fd0a9b96f759c3af6e6944d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015594"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Settings().ResetToDefault().Post(options)


```