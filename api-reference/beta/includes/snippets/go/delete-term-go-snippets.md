---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 920fee8b5d718533007ad2a929969c69c42718b1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033613"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

setId := "set-id"
termId := "term-id"
graphClient.TermStore().SetsById(&setId).TermsById(&termId).Delete(options)


```