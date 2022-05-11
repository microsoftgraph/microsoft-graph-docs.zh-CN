---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3822e7b9699c119e7999c7047088b6b924bf1453
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328446"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contractId := "contract-id"
result, err := graphClient.ContractsById(&contractId).Get()


```