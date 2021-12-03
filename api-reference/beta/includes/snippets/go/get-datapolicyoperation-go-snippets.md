---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06e99f551e002661b3406f576a352741017d1220
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287839"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

dataPolicyOperationId := "dataPolicyOperation-id"
result, err := graphClient.DataPolicyOperationsById(&dataPolicyOperationId).Get(nil)


```