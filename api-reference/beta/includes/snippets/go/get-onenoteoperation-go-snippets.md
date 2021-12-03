---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 893b5aec11e5503c19a0a701eadc788be6b847b5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288670"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

onenoteOperationId := "onenoteOperation-id"
result, err := graphClient.Me().Onenote().OperationsById(&onenoteOperationId).Get(nil)


```