---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3d690cf135f9196d4cb14fdd3dc85cba2ef56bc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032906"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printConnectorId := "printConnector-id"
graphClient.Print().ConnectorsById(&printConnectorId).Delete(options)


```