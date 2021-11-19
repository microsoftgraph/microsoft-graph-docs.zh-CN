---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0949cb2d1ba6870fed3b17c5bbd69a6b14e30c9c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089894"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

caseId := "case-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSourcesById(&noncustodialDataSourceId).Get(options)


```