---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ed7959b4965d3c9d4efd9b35c12b847c14879b6
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288601"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

webAccountId := "webAccount-id"
graphClient.Me().Profile().WebAccountsById(&webAccountId).Delete(nil)


```