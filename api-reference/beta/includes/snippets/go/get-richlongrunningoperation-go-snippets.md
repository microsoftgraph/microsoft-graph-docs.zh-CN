---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70b3ea726548a408a552a8c61db612cfdb87a9b6
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
richLongRunningOperationId := "richLongRunningOperation-id"
result, err := graphClient.SitesById(&siteId).OperationsById(&richLongRunningOperationId).Get(nil)


```