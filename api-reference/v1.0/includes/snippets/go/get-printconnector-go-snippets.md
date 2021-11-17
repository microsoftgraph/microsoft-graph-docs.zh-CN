---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53e492af8d0b89e30380e665900200bf17ac04e9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027200"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

printConnectorId := "printConnector-id"
result, err := graphClient.Print().ConnectorsById(&printConnectorId).Get(options)


```