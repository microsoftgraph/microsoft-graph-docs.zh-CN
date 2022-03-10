---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 804852694e20b2454f259a72072e6c21224142d9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411758"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Reopen(case-id).Post(nil)


```