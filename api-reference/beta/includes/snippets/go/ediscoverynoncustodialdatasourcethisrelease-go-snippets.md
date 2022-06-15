---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5448bd17a7730fd24822ff3a1fbfba23b04bdc5c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092203"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryNoncustodialDataSourceId := "ediscoveryNoncustodialDataSource-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSourcesById(&ediscoveryNoncustodialDataSourceId).Release(ediscoveryCase-id, ediscoveryNoncustodialDataSource-id).Post()


```