---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98a679cc69f8b3c63d76e3136d5f7aa1d7641956
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryCase()
displayName := "My Case 1 - Renamed"
requestBody.SetDisplayName(&displayName)
description := "Updated description"
requestBody.SetDescription(&description)
ediscoveryCaseId := "ediscoveryCase-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Patch(requestBody)


```