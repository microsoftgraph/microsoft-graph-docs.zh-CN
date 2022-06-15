---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a1563fb57e3f65488c8d7660d5ec3def06bc9eb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewTagId := "ediscoveryReviewTag-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).TagsById(&ediscoveryReviewTagId).Get()


```