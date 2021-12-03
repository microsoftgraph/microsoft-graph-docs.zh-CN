---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72269733ea653d9700b1d90d49fde835f804e9dd
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287490"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemEmailId := "itemEmail-id"
graphClient.Me().Profile().EmailsById(&itemEmailId).Delete(nil)


```