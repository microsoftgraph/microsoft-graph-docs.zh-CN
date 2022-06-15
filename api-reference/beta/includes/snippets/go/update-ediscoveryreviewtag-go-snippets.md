---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6e2ffea5737b8bfd53b5403c6fa028860c69127
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093692"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryReviewTag()
displayName := "My tag API 2"
requestBody.SetDisplayName(&displayName)
description := "Use Graph API to create tags (updated)"
requestBody.SetDescription(&description)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewTagId := "ediscoveryReviewTag-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).TagsById(&ediscoveryReviewTagId).Patch(requestBody)


```