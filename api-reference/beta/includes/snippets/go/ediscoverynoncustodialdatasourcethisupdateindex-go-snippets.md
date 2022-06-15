---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb40ae98cffe9d4522cfd81529960a842f5fd0da
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092784"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryNoncustodialDataSourceId := "ediscoveryNoncustodialDataSource-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSourcesById(&ediscoveryNoncustodialDataSourceId).UpdateIndex(ediscoveryCase-id, ediscoveryNoncustodialDataSource-id).Post()


```