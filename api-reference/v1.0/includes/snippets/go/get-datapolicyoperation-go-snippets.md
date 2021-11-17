---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 176365e270b310e5e0436735c72c40483b8bdb7d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

dataPolicyOperationId := "dataPolicyOperation-id"
result, err := graphClient.DataPolicyOperationsById(&dataPolicyOperationId).Get(options)


```