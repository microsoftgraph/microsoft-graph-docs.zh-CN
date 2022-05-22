---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d8efdbc329065ac42ed378212a6a640a43e1349
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).NoncustodialSources().Get()


```