---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c3c28106c8fe7bacf361359575d80b2d68e66c7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337588"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewHistoryDefinitionId := "accessReviewHistoryDefinition-id"
accessReviewHistoryInstanceId := "accessReviewHistoryInstance-id"
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById(&accessReviewHistoryDefinitionId).InstancesById(&accessReviewHistoryInstanceId).GenerateDownloadUri().Post(nil)


```