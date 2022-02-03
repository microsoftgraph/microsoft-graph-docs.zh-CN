---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c3c28106c8fe7bacf361359575d80b2d68e66c7
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340553"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewHistoryDefinitionId := "accessReviewHistoryDefinition-id"
accessReviewHistoryInstanceId := "accessReviewHistoryInstance-id"
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById(&accessReviewHistoryDefinitionId).InstancesById(&accessReviewHistoryInstanceId).GenerateDownloadUri().Post(nil)


```