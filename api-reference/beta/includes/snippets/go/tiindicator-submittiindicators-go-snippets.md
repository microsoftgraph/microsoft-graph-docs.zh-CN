---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 778869a367910b3e98cf697726d5af06649a9e97
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288273"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Security().TiIndicators().SubmitTiIndicators().Post(nil)


```