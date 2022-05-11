---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e1234ad73bdb1445102766484587df5d9c733d6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326235"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

dataPolicyOperationId := "dataPolicyOperation-id"
result, err := graphClient.DataPolicyOperationsById(&dataPolicyOperationId).Get()


```