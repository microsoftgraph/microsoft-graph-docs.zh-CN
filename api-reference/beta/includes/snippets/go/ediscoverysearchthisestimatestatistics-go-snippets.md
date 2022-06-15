---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 798e2fb23a3ad4aef182e4d3c5f69e4d06235f4e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093994"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoverySearchId := "ediscoverySearch-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).SearchesById(&ediscoverySearchId).EstimateStatistics(ediscoveryCase-id, ediscoverySearch-id).Post()


```