---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 277d693fcf70ecbb2a6d44462aaf8779c7b19511
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094946"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSourcesById(&noncustodialDataSourceId).DataSource().Get(options)


```