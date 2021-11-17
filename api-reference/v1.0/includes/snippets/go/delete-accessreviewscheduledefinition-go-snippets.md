---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd308d98cc7ebeaaad98acfbaf4189bc27d73937
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).Delete(options)


```