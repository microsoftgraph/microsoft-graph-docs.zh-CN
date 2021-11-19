---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b730c24f8cc3aafeaa2204a049fffbabd0335e9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081617"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
tagId := "tag-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).TagsById(&tagId).Get(options)


```