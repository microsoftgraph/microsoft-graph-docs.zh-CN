---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cafbde8860c48525838f5c57a55a5a9e01d6c8a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoverySearchId := "ediscoverySearch-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).SearchesById(&ediscoverySearchId).Delete()


```