---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 748f8c69eb4240939bfde788fb13e54d6a1e1763
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992122"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewHistoryDefinitionId := "accessReviewHistoryDefinition-id"
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById(&accessReviewHistoryDefinitionId).GenerateDownloadUri().Post(options)


```