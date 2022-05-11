---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2492629172155ba7b6b94fd52c3dded6f4a1de2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326615"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printConnectorId := "printConnector-id"
graphClient.Print().ConnectorsById(&printConnectorId).Delete()


```