---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ca8e123cfef9cbeb71a7d994ded8352a171f253
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095750"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printConnectorId := "printConnector-id"
graphClient.Print().ConnectorsById(&printConnectorId).Delete(options)


```