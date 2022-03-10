---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8abee612ccea04e67f26dd3dbaba5a0f28b3007
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412383"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Close(case-id).Post(nil)


```