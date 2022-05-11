---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e88c63c0d9e63c41740ca2320aa47b622b92bae
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

siteId := "site-id"
richLongRunningOperationId := "richLongRunningOperation-id"
result, err := graphClient.SitesById(&siteId).OperationsById(&richLongRunningOperationId).Get()


```