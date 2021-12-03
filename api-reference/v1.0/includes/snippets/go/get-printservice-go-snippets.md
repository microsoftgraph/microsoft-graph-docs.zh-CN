---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55b99f3896c6c648f10a2eb5230e7a49c20ee294
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288011"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printServiceId := "printService-id"
result, err := graphClient.Print().ServicesById(&printServiceId).Get(nil)


```